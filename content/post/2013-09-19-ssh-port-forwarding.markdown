+++
categories = ["ssh"]
date = "2013-09-19T16:49:50-07:00"
draft = false
title = "SSH Port Forwarding"
slug = "ssh-port-forwarding"
tags = []
+++

In the course of developing and taking web applications for a test
drive, it can be handy to access non-standard ports on a machine
without making them accessible to anyone. In my case, port forwarding
over SSH was an effective solution.

## The Problem
A remote machine has a service available over a port (e.g. 8080) that
is not accessible from your current workstation (as a result of a
firewall or something similar). You've got SSH access to the machine.

## The Solution
In short:


    ssh <user>@<remote-host> -L <local-port>:<target-host>:<remote-target-port> -N

### Breaking it down
`-L` tells ssh to forward a port
locally.

`local-port` is the port that will be available on your local
workstation.

`target-host` is which machine hosts the service you're
trying to forward *as the remote machine sees it*. This would
typically be `localhost` if the service is hosted on the machine that
you're connecting to over SSH, but it could be different. In an
example that I've used before, I was actually forwarding a port that
was hosted on a VM. In this case, the machine I was connecting to over
SSH was not the same machine that I was forwarding a port from, and
`target-host` reflected an IP address that was local to the target machine.

`remote-target-port` is the port that the service is actually
available on (the port you'd like to forward).

`-N` tells `ssh` to block the input on this command. The result is
that this specific terminal is blocked on this command, and it's a
good reminder to close the SSH connection when you're done.

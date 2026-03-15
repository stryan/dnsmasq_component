# README

This is an example [Materia](https://primamateria.systems) component for installing and configuring [dnsmasq](https://thekelleys.org.uk/dnsmasq/doc.html) running in a container. It was written for my personal and instructional use; I would not recommend using it in production (though I am).

You can use it in your own Materia repository as a remote component like so:

```
      [Remotes.dnsmasq.git]
      URL = "https://github.com/stryan/dnsmasq_component"
```

This component was designed for Materia v0.6.0.

# Configuration via Attributes

By default this component sets up no configuration for dnsmasq. The following attributes are available for configuration:

- `containerTag`: what container tag to use. Defaults `latest`
- `hostPort `= What to interface/port to publish. Defaults to `53`
- `useSeperateFiles `= Whether to include the `hosts` and `ethers` files. Defaults to `true`
- `confContents `= The contents of the `dnsmasq.conf` file. Defaults to empty.
- `hosts `= The contents of the `/etc/hosts` file. Defaults to empty.
- `ethers `=  The contents of the `/etc/ethers` file. Defaults to empty.

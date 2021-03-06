Title: Install OpenStack from a bundle
TODO: Add link to downloadable bundle file

# Install OpenStack from a bundle

[Stepping through the deployment][installopenstack] of each OpenStack
application is the best way to understanding how OpenStack and Juju operate,
and how each application relates to one another. But it's a labour intensive
process.

A bundle allows you to accomplish the same deployment with a single command:

```bash
juju deploy openstack.bundle
```

A [bundle][bundle], as used above, encapsulates the entire deployment process,
including all applications, their configuration parameters and any relations
that need to be made. Generally, you can use a local file, as above, or deploy
a curated bundle from the [charm store][osbundle].

For our project, [download the OpenStack][downloadbundle] and deploy OpenStack
using the above command.

The speed of the deployment depends on your hardware, but may take some time.
Monitor the output of `juju status` to see when everything is ready.

## Next steps

See the [Install OpenStack][testopenstack] documentation for details on testing
your OpenStack deployment, or jump directly to 
[Configure OpenStack][openstackconfig] to start using OpenStack productively as
quickly as possible.

<!-- LINKS -->
[installopenstack]: ./install-openstack.md
[testopenstack]: ./install-openstack.md#test-openstack
[bundle]: https://jujucharms.com/docs/stable/charms-bundles
[osbundle]: ./install-openstack-bundle.md
[openstackconfig]: ./config-openstack.md

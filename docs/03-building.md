# Building and Contributing blocks
At their most basic, a block is simply a pre-built container that runs an executable to provide whatever the function of that block is. So it's perfectly possible to build your block with `docker build` or any other OCI container build tools. However, those tools put the maintenance burden on the developer. By building your blocks on the balena software stack, that burden is vastly reduced.

## Balena Push
Just as with a fleet, a block can be built using the balena builder, by using the [balena CLI](https://www.balena.io/docs/reference/balena-cli/) and performing a

```
balena push <blockname>
```

(more CLI docs [here](https://www.youtube.com/watch?v=ItFi_08B4wc))

Once built, you can then see and manage your block in balenaCloud:

![browser reference](https://raw.githubusercontent.com/balenablocks/blocks/master/docs/images/dashboard-browser.png)

You can use all of the [release management](https://www.balena.io/docs/learn/deploy/release-strategy/release-policy/) functionality to manage your block
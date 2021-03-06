<p align="center">
 <img src="https://user-images.githubusercontent.com/47108/53650191-fa1fa800-3c11-11e9-8a49-955ac98d3486.png" width="661" />
</p>

<p align="center">
  <a href="https://circleci.com/gh/ethereum/grid-ui"><img src="https://img.shields.io/circleci/project/github/ethereum/grid-ui/master.svg" alt="Build Status"></a>
</p>

## Grid UI

### Project Goals

- improved security and easier maintenance than former Mist
- rapid development, faster iterations and releases
- improved testability
- removal of electron API references from UI components
- allows to run the app in a browser, electron or [tau](https://github.com/PhilippLgh/tau) window
- separation of electron shell application and user interface
- independent release, versioning and packaging of host application (Grid) and dapp (Grid UI, Wallet UI)
- introduction of an app namespace and removal of global variables
- reducing the amount of custom build scripts required to produce distributables
- a popular technology to encourage the community to contribute
- no network connection or full node required to run and develop the UI

### Contributing

There are many ways to get involved with this project. Get started [here](/docs/CONTRIBUTING.md).

### Development

```
git clone https://github.com/ethereum/grid-ui.git
cd grid-ui
yarn

Start in 2 terminals:
yarn run start -> start dev server for react with hot reloading
yarn run electron:dev -> load the app from the dev server into an electron window
```

#### Using local ethereum-react-components

To develop in `grid-ui` using your local copy of `ethereum-react-components`:

1. cd `ethereum-react-components`
1. `npm link`
1. cd `grid-ui`
1. `npm link ethereum-react-components`

After making changes in `ethereum-react-components`, run `yarn` for a fresh build to be picked up by `grid-ui`.

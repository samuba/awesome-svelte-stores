# List of awesome Svelte stores
There are many very useful svelte stores that might make your life easier without you knowing that they exist. Hence this list to surface those gems.
Just reading through the list might also give you some inspiration for solving your problems more elegantly with a store. PR's welcome.

ℹ️ Many stores are just one small file that you can drop in your project without even having to add a dependency.


## Browser Storage
- [persistent-svelte-store](https://github.com/omer-g/persistent-svelte-store) 
  - Built from scratch in TypeScript. Is reactive across tabs or windows using the Broadcast Channel API.
- [@macfja/svelte-persistent-store](https://github.com/MacFJA/svelte-persistent-store)
  - Supports different/custom storage providers 
- [babichjacob/svelte-localstorage](https://github.com/babichjacob/svelte-localstorage)
  - SSR support 
- [@furudean/svelte-persistent-store](https://github.com/furudean/svelte-persistent-store) 
    - Saves and loads data from `Window.localStorage` or `Window.sessionStorage`.
- [LocalStorage Custom Store](https://svelte.dev/repl/e6c0e3db7d064d43a7e4559b2862e1f7?version=3.48.0)
  - Very simple persisting to localstorage.  

## Browser Navigation
- [svelte-store-router](https://github.com/zyxd/svelte-store-router) 
    - Router for Svelte that suggests that routing is just another global state and History API changes are just an optional side-effects of this state.
- [query-store](https://github.com/buhrmi/query-store )
    - Writable store that syncs with the browser's search param

## Fetching Data
- [svelte-query](https://github.com/SvelteStack/svelte-query)
  - Advanced asynchronous state management including caching, auto-refetching etc. TanStack/query fork?
- [svelte-asyncable](https://github.com/PaulMaly/svelte-asyncable )
    - Tiny, declarative, optimistic, async store
- [Fetch Store](https://svelte.dev/repl/a74f1ed8e3eb4aec82cb743e13443ee4?version=3.48.0)
  - Convenience wrapper for `fetch()`
- [Periodic Fetch Store](https://svelte.dev/repl/b8fa406464d6434fba97902ac78b5e2b?version=3.48.0)
- [svelte-websocket-store](https://github.com/arlac77/svelte-websocket-store)
  - Send/receive data from a websocket 
- [@macfja/svelte-invalidable](https://github.com/MacFJA/svelte-invalidable )
    - A store that can be requested to update itself

## Undo
- [storez](https://github.com/plrenaudin/svelte-storez )
    - Writable store with old/new value, change history + undo, debounce, localstorage persist
- [@macfja/svelte-undoable](https://github.com/macfja/svelte-undoable )
    - Memento design pattern (undo/redo) in Svelte
- [svelte-previous](https://github.com/bryanmylee/svelte-previous) 
    - Remember previous values - helpful for transitions or a quick undo stack

## Upgraded Stores
- [@macfja/svelte-expirable](https://github.com/MacFJA/svelte-expirable )
    - A Svelte store with items that expire
- [svelte-store2](https://github.com/vkurko/svelte-store2 )
    - Adds a `get()` function to writable, derived and readable that returns the actual value without subscribing/ubsubscribing in the background like svelte's normal [get()]
    (https://svelte.dev/docs#run-time-svelte-store-get) function.
- [SvelteStore](https://github.com/gitbreaker222/SvelteStore )
    - Track state diffs, Inspect current state, Type warnings, Persistent storage, Infinite loop detection, Testable Actions, Audible activity

## Stores affecting each other
- [svelte-keyed](https://github.com/bryanmylee/svelte-keyed) 
    - Takes a writable object store and a keypath, and returns a writable store whose changes are reflected on the original store. Properties are accessed with dot notation, and arrays can be indexed with bracket notation.
- [Svelte-nStore](https://github.com/lacikawiz/svelte-nStore) 
    - Adds `get()` without subsription and recalculation of store value that is dependent on other stores values
- [svelte-writable-derived](https://github.com/PixievoltNo1/svelte-writable-derived )
    - Two-way data-transforming store

## State Machine
- [svelte-fsm](https://github.com/kenkunz/svelte-fsm)
  - Only 1kb, very simple, typescript support
  - [9min video introduction](https://www.youtube.com/watch?v=3_D-3HPUdEI)
- [xstate-svelte](https://xstate.js.org/docs/packages/xstate-svelte/#quick-start)
  - Wrapper around [xstate](https://xstate.js.org/). Xstate: 30kb, complete suit with visual editor and support for charts.
  - [7min video introduction](https://www.youtube.com/watch?v=NIfQsc5XAzU)
- [svate](https://github.com/AlexxNB/svate )
    - Set of simple state machines for Svelte application (Flag, Flagset..)

## (Im)mutability
- [svelte-mutable-store](https://github.com/feltcoop/svelte-mutable-store) 
    - Mutable values when using  the  svelte `immutable` compiler option
- [svelte-restate](https://github.com/endenwer/svelte-restate )
    - Immutable store for Svelte with full Typescript support and Redux Devtools integration
- [svelte-readonly](https://github.com/Crisfole/svelte-readonly) 
    - Very small store that exposes only a readable interface.

## Inspired State Management
- [stores-x](https://github.com/Anyass3/stores-x) 
    - State management heaviliy inspired by [VueX](https://github.com/vuejs/vuex)
- [MiniRx](https://spierala.github.io/mini-rx-store/) 
    - RxJS Redux Store that works with TypeScript

## CSS
- [sw-yx/everything-store](https://github.com/sw-yx/everything-store)
  - CSS related stores for: Tailwind Breakpoints, Media Queries, Dark Mode 
- [svelte-animation-store](https://github.com/joshnuss/svelte-animation-store) 
    - Based on Svelte's tweened store, that lets you pause, continue, reset, replay, reverse or adjust speed of a tween.

## Notifications
- [Notification Toast Custom Store](https://svelte.dev/repl/e166b01bc46149a49895c1622d26ce7e?version=3.48.0)
  - Auto-disappearing notifications/toasts

## 3rd-Party interaction
- [svelte-ethers-store](https://www.npmjs.com/package/svelte-ethers-store) 
    - ethers.js to interact with the Ethereum Blockchain

## Others
- [timhall/svelte-observable](https://github.com/timhall/svelte-observable)
  - Wrapper for Observables (e.g. RxJS) 
- [Toggle Store](https://svelte.dev/repl/a3cb054398a94698a4cfe4c44f33b923?version=3.48.0)
- [svelte-webext-storage-adapter](https://github.com/PixievoltNo1/svelte-webext-storage-adapter )
    - Writable stores for Firefox/Chrome extensions using `chrome.storage
- [svelte-lens-store](https://github.com/aredridel/svelte-lens-store) 
    - Functional lenses over Svelte stores
- [svelte-xactor](https://github.com/wobsoriano/svelte-xactor) 
    - Middleware that allows you to easily convert your xactor actors (actors from [xstate](https://xstate.js.org/)) into a global store
- [svelte-damped-store](https://github.com/aredridel/svelte-damped-store) 
    - derived writable store that can suspend updates while user is still interacting 
- [svelte-entity-store](https://github.com/tony-sull/svelte-entity-store) 
    -  Simple, generic solution for storing collections of entity objects.

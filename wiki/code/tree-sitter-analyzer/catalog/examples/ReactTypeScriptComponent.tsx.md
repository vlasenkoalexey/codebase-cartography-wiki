---
title: 'Module: examples/ReactTypeScriptComponent.tsx'
type: catalog
provenance: extracted
module: examples/ReactTypeScriptComponent.tsx
status: fresh
symbol_base: scip-typescript npm . . examples/`ReactTypeScriptComponent.tsx`/
symbols:
  App: App.
  AppProvider: AppProvider.
  UserManager.render: UserManager#render().
  UserManager.loadUsers: UserManager#loadUsers.
  User: User#
  Button: Button.
  UserForm: UserForm.
  useApi.typeLiteral581.refetch: useApi().typeLiteral581:refetch.
  Counter.render: Counter#render().
  UserList: UserList.
  UserManager.handleFormSubmit: UserManager#handleFormSubmit.
  FormData: FormData#
  Counter.defaultProps: Counter#defaultProps.
  useAppContext: useAppContext.
  Counter: Counter#
  User.id: User#id.
  AppRoot: AppRoot.
  AppContext: AppContext.
  User.role: User#role.
  FormData.role: FormData#role.
  Counter.-constructor: Counter#`<constructor>`().
  UserCard: UserCard.
  UserManager: UserManager#
  User.name: User#name.
  Theme: Theme#
  AppContextType: AppContextType#
  UserManager.abortController: UserManager#abortController.
  AppContextType.user: AppContextType#user.
  AppContextType.theme: AppContextType#theme.
  UserManagerState: UserManagerState#
  UserManager.handleUserEdit: UserManager#handleUserEdit.
  User.email: User#email.
  CounterProps: CounterProps#
  CounterProps.initialCount: CounterProps#initialCount.
  useLocalStorage: useLocalStorage().
  AppContextType.setUser: AppContextType#setUser.
  AppContextType.setTheme: AppContextType#setTheme.
  ButtonProps.variant: ButtonProps#variant.
  ButtonProps.size: ButtonProps#size.
  UserCardProps.user: UserCardProps#user.
  UserCardProps.onEdit: UserCardProps#onEdit.
  UserListProps.users: UserListProps#users.
  UserListProps.onUserSelect: UserListProps#onUserSelect.
  UserListProps.onUserEdit: UserListProps#onUserEdit.
  UserFormProps.initialData: UserFormProps#initialData.
  UserFormProps.onSubmit: UserFormProps#onSubmit.
  UserManagerState.users: UserManagerState#users.
  UserManager.componentDidMount: UserManager#componentDidMount().
  UserManager.componentWillUnmount: UserManager#componentWillUnmount().
  Theme.background: Theme#background.
  Theme.text: Theme#text.
  ButtonVariant: ButtonVariant#
  Size: Size#
  ButtonProps: ButtonProps#
  UserCardProps: UserCardProps#
  UserListProps: UserListProps#
  FormData.email: FormData#email.
  UserFormProps: UserFormProps#
  CounterProps.step: CounterProps#step.
  useApi: useApi().
  useApi.typeLiteral581.data: useApi().typeLiteral581:data.
  useApi.typeLiteral581.loading: useApi().typeLiteral581:loading.
  useApi.typeLiteral581.error: useApi().typeLiteral581:error.
  User.avatar: User#avatar.
  Theme.primary: Theme#primary.
  Theme.secondary: Theme#secondary.
  FormData.name: FormData#name.
  UserManager.handleUserDelete: UserManager#handleUserDelete.
  UserManager.handleFormCancel: UserManager#handleFormCancel.
  UserManager.handleAddUser: UserManager#handleAddUser.
  CounterProps.onCountChange: CounterProps#onCountChange.
  CounterState: CounterState#
  Counter.increment: Counter#increment.
  Counter.decrement: Counter#decrement.
  Counter.reset: Counter#reset.
  AppProviderProps: AppProviderProps#
  ButtonProps.disabled: ButtonProps#disabled.
  ButtonProps.loading: ButtonProps#loading.
  ButtonProps.onClick: ButtonProps#onClick.
  ButtonProps.children: ButtonProps#children.
  ButtonProps.className: ButtonProps#className.
  ButtonProps.style: ButtonProps#style.
  UserCardProps.onDelete: UserCardProps#onDelete.
  UserCardProps.showActions: UserCardProps#showActions.
  UserListProps.loading: UserListProps#loading.
  UserListProps.error: UserListProps#error.
  UserListProps.onUserDelete: UserListProps#onUserDelete.
  UserFormProps.onCancel: UserFormProps#onCancel.
  UserFormProps.loading: UserFormProps#loading.
  UserManagerState.loading: UserManagerState#loading.
  UserManagerState.error: UserManagerState#error.
  UserManagerState.showForm: UserManagerState#showForm.
  UserManagerState.editingUser: UserManagerState#editingUser.
  UserManager.-constructor: UserManager#`<constructor>`().
  CounterState.count: CounterState#count.
  AppProviderProps.children: AppProviderProps#children.
---
# Module: [`examples/ReactTypeScriptComponent.tsx`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx)

## Classes
### `AppContextType`
- def: [`examples/ReactTypeScriptComponent.tsx:49`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L49)
- signature: `interface AppContextType`
- members:
  - `setTheme` — [`L53`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L53)
  - `setUser` — [`L52`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L52)
  - `theme` — [`L51`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L51)
  - `user` — [`L50`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L50)
- uses (calls/refs, reference-scoped): (2 test-only callers)
- used by: (5 test-only callers)

### `AppProviderProps`
- def: [`examples/ReactTypeScriptComponent.tsx:766`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L766)
- signature: `interface AppProviderProps`
- members:
  - `children` — [`L767`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L767)
- used by: (1 test-only callers)

### `ButtonProps`
- def: [`examples/ReactTypeScriptComponent.tsx:69`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L69)
- signature: `interface ButtonProps`
- members:
  - `children` — [`L75`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L75)
  - `className` — [`L76`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L76)
  - `disabled` — [`L72`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L72)
  - `loading` — [`L73`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L73)
  - `onClick` — [`L74`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L74)
  - `size` — [`L71`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L71)
  - `style` — [`L77`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L77)
  - `variant` — [`L70`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L70)
- uses (calls/refs, reference-scoped): (2 test-only callers)
- used by: (1 test-only callers)

### `ButtonVariant`
- def: [`examples/ReactTypeScriptComponent.tsx:44`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L44)
- signature: `type ButtonVariant`
- used by: (2 test-only callers)

### `Counter`
- def: [`examples/ReactTypeScriptComponent.tsx:615`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L615)
- doc: パフォーマンス最適化されたカウンターコンポーネント
- signature: `class Counter`
- members:
  - `<constructor>(props: CounterProps)` — [`L621`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L621) — パフォーマンス最適化されたカウンターコンポーネント
  - `render(method)` — [`L652`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L652)
  - `decrement` — [`L636`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L636)
  - `defaultProps` — [`L616`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L616)
  - `increment` — [`L628`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L628)
  - `reset` — [`L644`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L644)
- uses (calls/refs, reference-scoped): (5 test-only callers)
- used by: (2 test-only callers)

### `CounterProps`
- def: [`examples/ReactTypeScriptComponent.tsx:601`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L601)
- signature: `interface CounterProps`
- members:
  - `initialCount` — [`L602`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L602)
  - `onCountChange` — [`L604`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L604)
  - `step` — [`L603`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L603)
- used by: (4 test-only callers)

### `CounterState`
- def: [`examples/ReactTypeScriptComponent.tsx:607`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L607)
- signature: `interface CounterState`
- members:
  - `count` — [`L608`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L608)
- used by: (1 test-only callers)

### `FormData`
- def: [`examples/ReactTypeScriptComponent.tsx:96`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L96)
- signature: `interface FormData`
- members:
  - `email` — [`L98`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L98)
  - `name` — [`L97`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L97)
  - `role` — [`L99`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L99)
- uses (calls/refs, reference-scoped): (2 test-only callers)
- used by: (5 test-only callers)

### `Size`
- def: [`examples/ReactTypeScriptComponent.tsx:45`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L45)
- signature: `type Size`
- used by: (2 test-only callers)

### `Theme`
- def: [`examples/ReactTypeScriptComponent.tsx:37`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L37)
- signature: `interface Theme`
- members:
  - `background` — [`L40`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L40)
  - `primary` — [`L38`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L38)
  - `secondary` — [`L39`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L39)
  - `text` — [`L41`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L41)
- used by: (5 test-only callers)

### `User`
- def: [`examples/ReactTypeScriptComponent.tsx:29`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L29)
- signature: `interface User`
- members:
  - `avatar` — [`L33`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L33)
  - `email` — [`L32`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L32)
  - `id` — [`L30`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L30)
  - `name` — [`L31`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L31)
  - `role` — [`L34`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L34)
- used by: (18 test-only callers)

### `UserCardProps`
- def: [`examples/ReactTypeScriptComponent.tsx:80`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L80)
- signature: `interface UserCardProps`
- members:
  - `onDelete` — [`L83`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L83)
  - `onEdit` — [`L82`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L82)
  - `showActions` — [`L84`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L84)
  - `user` — [`L81`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L81)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `UserFormProps`
- def: [`examples/ReactTypeScriptComponent.tsx:102`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L102)
- signature: `interface UserFormProps`
- members:
  - `initialData` — [`L103`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L103)
  - `loading` — [`L106`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L106)
  - `onCancel` — [`L105`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L105)
  - `onSubmit` — [`L104`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L104)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `UserListProps`
- def: [`examples/ReactTypeScriptComponent.tsx:87`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L87)
- signature: `interface UserListProps`
- members:
  - `error` — [`L90`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L90)
  - `loading` — [`L89`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L89)
  - `onUserDelete` — [`L93`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L93)
  - `onUserEdit` — [`L92`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L92)
  - `onUserSelect` — [`L91`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L91)
  - `users` — [`L88`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L88)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `UserManager`
- def: [`examples/ReactTypeScriptComponent.tsx:430`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L430)
- doc: ユーザー管理クラスコンポーネント
- signature: `class UserManager`
- members:
  - `<constructor>(props: {})` — [`L433`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L433) — ユーザー管理クラスコンポーネント
  - `componentDidMount(method)` — [`L444`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L444)
  - `componentWillUnmount(method)` — [`L448`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L448)
  - `render(method)` — [`L557`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L557)
  - `abortController` — [`L431`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L431)
  - `handleAddUser` — [`L553`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L553)
  - `handleFormCancel` — [`L549`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L549)
  - `handleFormSubmit` — [`L512`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L512)
  - `handleUserDelete` — [`L499`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L499)
  - `handleUserEdit` — [`L495`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L495)
  - `loadUsers` — [`L454`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L454)
- uses (calls/refs, reference-scoped): (11 test-only callers)
- used by: (2 test-only callers)

### `UserManagerState`
- def: [`examples/ReactTypeScriptComponent.tsx:418`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L418)
- signature: `interface UserManagerState`
- members:
  - `editingUser` — [`L423`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L423)
  - `error` — [`L421`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L421)
  - `loading` — [`L420`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L420)
  - `showForm` — [`L422`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L422)
  - `users` — [`L419`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L419)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

## Functions
- `useApi(url: string, options?: RequestInit)` — [`L723`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L723) — API呼び出し用カスタムフック
- `useLocalStorage(key: string, initialValue: T)` — [`L692`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L692) — ローカルストレージを使用するカスタムフック

## Module values
- `App` — [`L803`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L803) — メインアプリケーションコンポーネント
- `AppContext` — [`L56`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L56)
- `AppProvider` — [`L774`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L774) — アプリケーションコンテキストプロバイダー
- `AppRoot` — [`L887`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L887) — アプリケーションのルートコンポーネント
- `Button` — [`L115`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L115) — 再利用可能なボタンコンポーネント
- `UserCard` — [`L158`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L158) — ユーザーカードコンポーネント
- `UserForm` — [`L231`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L231) — ユーザーフォームコンポーネント
- `UserList` — [`L356`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L356) — ユーザーリストコンポーネント
- `data` — [`L727`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L727)
- `error` — [`L729`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L729)
- `loading` — [`L728`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L728)
- `refetch` — [`L730`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L730)
- `useAppContext` — [`L59`](../../../../../raw/code/tree-sitter-analyzer/examples/ReactTypeScriptComponent.tsx#L59)


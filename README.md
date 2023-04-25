# React and Typescript: Build a Portfolio Project

Hi, It's me (Hoang Le), one more time, I go even deeper in ReactJS. And this repository contains the code of the [React and Typescript: Build a Portfolio Project
](https://www.udemy.com/course/react-and-typescript-build-a-portfolio-project/).

**Most focus in folder redux-ts**

Some notes:

Explicit component type annotations: React.FC<props interface>. If using React.FC we will have benefit:

Component will be a React function component

Component might have properties assigned to it like ‘propTypes’ and ‘contextTypes’

Component will receive props of type ‘ChildProps’ (interface of props)

---

State with typescript: useState<interface>

---

- Handle input event:

const onChange = (event: React.ChangeEvent<HTMLInputElement>) => {};

- Using useRef with typscript:

const inputRef = useRef<HTMLInputElement | null>(null);
useEffect(() => {
inputRef.current?.focus();
}, []);

- Typescript with class components

---

API: http://registry.npmjs.org/-/v1/search?text=react

- Call NPM packages: repositories. Because it's a sensitive word.

- useSelector = mapStateToProps

- Setup redux with typescript: reducers, actions, action-types, action-creators.

- Using 1 file state\index.ts to export all that need from the state. Instead of, import file by file in components.

- Using custom hook:

- useAction: useDispatch to dispatch actions.

- useTypedSelector: useSelector to get state.

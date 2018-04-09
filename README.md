# Code Editor

[Show me the demo!](https://patilvg89.github.io/)

### Run Locally

```
  npm install
  npm start // visit localhost:8080
```

### Sample Code

const reducer = (state=[], action) => {
	if( action.type === 'split_string'){
		return action.payload.split('');	
	}
  return state;
};

const action = {
	type:'split_string',
  payload: 'abcdef'
}

const store = Redux.createStore(reducer);

store.dispatch(action)

store.getState()

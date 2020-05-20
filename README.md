# componentDidMount

### Correct way of writing componentDidMount to prevent re-render of component or action.

```
componentDidUpdate(prevProps) {
    if (prevProps.systemId !== this.props.systemId) {
      this.props.getUserMenuList(this.props.systemId, this.props.token);
    }
  }
```

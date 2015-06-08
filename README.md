#react size decorator, 
adds width and height props to component
(*also recalculates this props on resize*)

#install
```bash
npm install --save size-decorator
```

#usage
```javascript
import size from 'size-decorator';
@size()
export default class MySuperComponent extends Component {
  constructor(props) {
    super(props);
  }

  render() {
    console.log(this.props.width, this.props.height)
    return (<div style={{width: 100, height: 100}}>HELLO</div>);
  }
}
```

or if you want width and height parameters on server

```javascript
@size({width: 100, height: 200})
```



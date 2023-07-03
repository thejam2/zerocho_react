# zerocho_react

## 클래스형 컴포넌트 구조
```
class 클래스명 extends React.Component {
    constructor(props) {
      super(props);
      this.state = {liked: false}; //state
    }

    render() {
      if (this.state.liked) {
        return 'You liked this.';
      }

      return (
        <button onClick={() => this.setState({liked: true})}>
          Like
        </button>
      );
    }
  }
```

## 함수형 컴포넌트 구조
```
const 클래스명 = ()=>{
    const [state, setState] = React.useState(false);

    return (
        <button onClick={() => setState(true)}>
          Like
        </button>
    )
}
```

## Node
Node는 자바스크립트 실행기 

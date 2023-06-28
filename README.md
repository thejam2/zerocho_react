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

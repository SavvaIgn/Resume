
<html>
<head>
<header>Hi! My name is Savva Ignatov<header><br>
</head>
<div id="like_button_container"></div>
'use strict';

const e = React.createElement;

class LikeButton extends React.Component {
  constructor(props) {
    super(props);
    this.state = { liked: false };
  }

  render() {
    if (this.state.liked) {
      return 'You liked this.';
    }

    return e(
      'button',
      { onClick: () => this.setState({ liked: true }) },
      'Like'
    );
  }
}
const domContainer = document.querySelector('#like_button_container');
const root = ReactDOM.createRoot(domContainer);
root.render(e(LikeButton));
<li>I'm a Harvey Mudd College student expected to graduate in 2025
<li>Here are some projects I have worked on: https://github.com/SavvaIgn/projects-for-resume.git
<li>Here is a snake game I worked on if you want to play: https://github.com/SavvaIgn/Snake-Game.git<br>

<header>Coding Languages<header>

<li>Python
<li>Java
<li>C++
<li>Racket<br>

<header>You can reach me here:<header><br>
+1 909-847-3567 | signatov@hmc.edu	| https://www.linkedin.com/in/savva-ignatov/
<script src="https://unpkg.com/react@18/umd/react.development.js" crossorigin></script>
<script src="https://unpkg.com/react-dom@18/umd/react-dom.development.js" crossorigin></script>

<script src="like_button.js"></script>
<body>





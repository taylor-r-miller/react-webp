# react-webp
React hook for detecting if a browser supports webp.

Lightweight package for determining if a browser supports webp images. Particularly helpful in creating fallbacks for background images without having to download a package with a size larger than the savings a webp image can provide. Examples at https://github.com/taylor-r-miller/react-webp.

To run example clone repo, cd into examples and run yarn start

Example:

import useWebp  from 'react-use-webp';

const App = () => {

  const { supportsWebP } = useWebp()


  return (
    <div className={supportsWebP ? 'bg-webp' : 'bg-jpg'}>
      {`Background image is ${supportsWebP ? 'webp' : 'jpg'}` }
    </div>
  );
};

ReactDOM.render(<App />, document.getElementById('root'));

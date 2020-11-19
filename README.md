# react-webp
React hook for detecting if a browser supports webp images.

Install- npm i react-use-webp

Lightweight package for determining if a browser supports webp images. Particularly helpful in creating fallbacks for background images without having to download a package with a size larger than the savings a webp image can provide. Examples at https://github.com/taylor-r-miller/react-webp.

To run example clone repo, cd into examples and run yarn start

Example:


import useWebp  from 'react-use-webp';

const { supportsWebP } = useWebp()

supportsWebp is boolean and can be used with a turnary to return differernt classNames in this example you would have two css classes one named webp-background and another named jpg-background each serving a background image of the respective type

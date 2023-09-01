# EliteCodeForge

## To create react app using vite

npm create vite@latest ./ -- --template react

## To install tailwind css

npm install -D tailwindcss postcss autoprefixer

/* since we are installing legacy version */

npm install --legacy-peer-deps -D tailwindcss postcss autoprefixer

## To initialize tailwindcss

npx tailwindcss init -p

## Additional packages

npm install --leagacy-peer-deps @react-three/fiber @react-three/drei maath react-tilt react-vertical-timeline-component @emailjs/browser framer-motion react-router-dom

## Installing original threejs

npm install --legacy-peer-deps three

## Aditional helping comments

1. Keep the file extension of postcss.config and tailwind.config as cjs instead of js

2. In tailwind.config.cjs keep 
export default {} instead of 
module.exports = {}

3. In postcss.config.cjs change 
export default {} to 
module.exports = {
  plugins: {
      tailwindcss: {},
      autoprefixer: {},
  }
}

4. A common error is using 
import Tilt from ""; instead of
import { Tilt } from "";
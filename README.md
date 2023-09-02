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

## Setting up emailjs service

1. Create an account on emailjs.com
2. Add new service
3. Click gmail
4. Connect your account
5. Sign in with gmail
6. Create service
7. Go to email template
8. Leave everything as it is and click save
9. Go to your template -> settings 
10. copy template id
11. Go to email services and click Gmail
12. Copy service id
13. Go to your name
14. Copy public key
15. Update these values in contact.jsx

## How to change icons and images

1. Go to assets 
2. Change the fie you want to change
3. Go to index.js in assets folder
4. Change import Your_File_Name from "File address"
5. Change export to your_file_name
6. Go to constants/index.js
7. Change the content accordingly
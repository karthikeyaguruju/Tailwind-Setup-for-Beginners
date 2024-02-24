--> Install Tailwind CSS:
1) npm install -D tailwindcss
2) npx tailwindcss init

--> Configure your template paths:

/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ["./src/**/*.{html,js}"],
  theme: {
    extend: {},
  },
  plugins: [],
}

--> Add the Tailwind directives to your CSS:
@tailwind base;
@tailwind components;
@tailwind utilities;

--> Start the Tailwind CLI build process:
npx tailwindcss -i ./src/input.css -o ./src/output.css --watch

--> Start using Tailwind in your HTML:
<!doctype html>
<html>
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <link href="./output.css" rel="stylesheet">
</head>
<body>
  <h1 class="text-3xl font-bold underline">
    Hello world!
  </h1>
</body>
</html>


==> Reference Links::
https://tailwindcss.com/docs/installation
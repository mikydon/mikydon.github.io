# mikydon.github.io

The root of https://mikydon.github.io. It only exists for two things:

- `.well-known/assetlinks.json`: Android App Links for [HW App](https://github.com/mikydon/hw-app). It tells Android that
  links like `https://mikydon.github.io/hw-app/add/?c=CODE` (a friend's invite) may open the app directly.
  Listed apps: `io.github.mikydon.hwapp` (release key) and `io.github.mikydon.hwapp.test` (the public debug key of the test build).
- `index.html`: sends visitors of the bare domain to https://mikydon.github.io/hw-app/.

`.nojekyll` makes GitHub Pages serve the `.well-known` folder (Jekyll skips folders that start with a dot).

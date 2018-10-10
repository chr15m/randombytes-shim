Tiny shim for `crypto.randomBytes(size);` for nodejs & browsers.

`npm i randombytes-shim`

Uses crypto / msCrypto implementations where available and falls back to using `Math.random()` in the worst case (e.g. IE11).

	> var randomBytes = require("randombytes-shim");
	> console.log(randombytes(3));
	Uint8Array [ 216, 210, 71 ]

Or `<script src="randombytes-shim.min.js"></script>` directly in your HTML.

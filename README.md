Lollagram - Instagram Real Time App
=============

## Intro

A real-time responsive "picture wall" that streams images from Instagram for specific hashtags.

This is a fork of [`instagram-real-time` by weblancaster](https://github.com/weblancaster/instagram-real-time).

## Original intro

From the [original repository](https://github.com/weblancaster/instagram-real-time#intro):

> To learn a little bit more of NodeJS, Socket.IO and for fun I developed the new version of Lollagram
consuming Instagram Real Time API.

> Feel free to ask me anything and I will do my best to answer any question.

> Lollagram is a labor of love that’s designed to help you keep track of the Lollapalooza experience, through the eyes (or, more accurately, snapshots) of music lovers on the ground at Grant Park. Lollagram takes advantage of the Instagram Real Time API and aggregates the moments at Lollapalooza, creating a visual record of the bands, food, people, and city that make up this great musical tradition. With 45 million photos being uploaded to Instagram each day, we're excited to present snapshots from Lollapalooza 2013.

> detailed blog post on <a href="http://www.bymichaellancaster.com/blog/how-i-built-lollagram-lollapalooza-instagram-real-time-api/" title="blog post" target="_blank">my website</a>

> Simple step-by-step checking <a href="http://git.io/Ry1fEA" title="step by step" target="_blank">http://git.io/Ry1fEA</a>

## Technologies

* Node.js
* Express.js
* Socket.io
* Handlebars

## Configuration

All configuration happens through either environment variables or the [`.env file`](https://www.npmjs.com/package/dotenv-node).

* `INSTAGRAM_CLIENT_ID`: Your ID for the Instagram API.
* `INSTAGRAM_CLIENT_SECRET`: Your secret key for the Instagram API.
* `BASE_URL`: The base URL that your application runs at. This must be publicly routable - the Instagram API will push updates to it!
* `SUBSCRIBE_TAGS`: A comma-delimited list of tags (without the `#`) to stream. The first tag will be considered the 'main' one, and used to "seed" the page on first load.
* `PORT`: The port to run on. Use [`authbind`](https://thomashunter.name/blog/using-authbind-with-node-js/) to run on privileged ports (eg. 80).

## Author

Original by Michael Lancaster, some modifications by Sven Slootweg.

## License

MIT

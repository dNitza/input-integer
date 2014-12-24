# &lt;input-integer&gt;

> A more usable integer input

## Demo

[Check it live!](http://dNitza.github.io/input-integer)

## Install

Install the component using [Bower](http://bower.io/):

```sh
$ bower install input-integer --save
```

Or [download as ZIP](https://github.com/dNitza/input-integer/archive/master.zip).

## Usage

1. Import Web Components' polyfill:

    ```html
    <script src="bower_components/webcomponentsjs/webcomponents.min.js"></script>
    ```

2. Import Custom Element:

    ```html
    <link rel="import" href="bower_components/input-integer/dist/input-integer.html">
    ```

3. Start using it!

    ```html
    <input-integer></input-integer>
    ```

## Options

Attribute     | Options     | Default      | Description
---           | ---         | ---          | ---
`min`         | *string*    | `infinity`        | The minimum value of the field
`max`         | *string*    | `infinity`        | The maximum value of the field.
`name`         | *string*    | ``        | The name of the field.
`value`         | *string*    | ``        | The value of the field.
`pattern`         | *string*    | ``        | The pattern this field must adhere to in order to be valid.

## Methods

Method        | Parameters   | Returns     | Description
---           | ---          | ---         | ---
`increment()`   | None.        | Nothing.    | Increments the value of the field by 1.
`decrement()`   | None.        | Nothing.    | Decrements the value of the field by 1.

## Events

Event         | Description
---           | ---
`on-scroll` | Increments or decrements depending on scroll direction.
`on-keydown` | Increments when up is pressed, decrements when down is pressed.

## Development

In order to run it locally you'll need to fetch some dependencies and a basic server setup.

* Install [Bower](http://bower.io/) & [Grunt](http://gruntjs.com/):

    ```sh
    $ [sudo] npm install -g bower grunt-cli
    ```

* Install local dependencies:

    ```sh
    $ bower install && npm install
    ```

* To test your project, start the development server and open `http://localhost:8000`.

    ```sh
    $ grunt server
    ```

* To build the distribution files before releasing a new version.

    ```sh
    $ grunt build
    ```

* To provide a live demo, send everything to `gh-pages` branch.

    ```sh
    $ grunt deploy
    ```

## Contributing

1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -m 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request :D

## History

For detailed changelog, check [Releases](https://github.com/dNitza/input-integer/releases).

## License

[MIT License](http://opensource.org/licenses/MIT)

# RaaS

This is a simple Sinatra application for generating and providing strings full
of random characters via HTTP.

## What?

Yeah, we know.  Deal with it.

## Disclaimer

This is a *proof of concept* and no guarantee is made to the fitness (or,
indeed, usefulness) of this application whatsoever.  Please enjoy responsibly.

## Requirements

 * Ruby v1.9.3 or better; anything less would be uncivilised.
 * The `sinatra` and `xml-simple` gems, along with other standard modules.

## Usage

So the API can deal with this : `/:enc/:charset/:len/:num`

 * Valid `:enc` are:
   * `p` for plain text
   * `j` for JSON
   * `y` for YAML
   * `h` for HTML
   * `x` for XML
 * Valid `:charset` are:
   * `ab` for basic alpha-numeric characters
   * `as` for "safe" alpha-numeric characters (no characters that are too similar visually)
   * `hex` for hexadecimal characters
   * `num` for numbers only
 * `:len` is length of each result
 * `:num` is the number of results

Run it like this : `$ ruby ./raas.rb`

## License

Released under the ASL 2.0; see `LICENSE` for details.

# nil_or

Delegates methods to the target unless nil.

## Getting started

    $ gem install nil_or

Or in your Gemfile:

    gem "nil_or"

## Usage

When x is not nil:

    x = 5
    x.nil_or.to_s
    => "5"
    x.nil_or + 2
    => 7
    x.nil_or.times { |i| puts i }
    ...

But when it is nil:

    x = nil
    x.nil_or.to_s
    => nil
    x.nil_r + 2
    => nil
    x.nil_or.shakalaka(1, 2) { does_nothing }
    => nil


# TangoSource Ruby Koans

The Ruby Koans walk you along the path to enlightenment in order to learn Ruby.
The goal is to learn the Ruby language, syntax, structure, and some common
functions and libraries. We also teach you culture. Testing is not just something we
pay lip service to, but something we live.  It is essential in your quest to learn
and do great things in the language.

## The Structure

The koans are broken out into areas by file, hashes are covered in about_hashes.rb,
modules are introduced in about_modules.rb, etc.  They are presented in order in the
path_to_enlightenment.rb file.

Each koan builds up your knowledge of Ruby and builds upon itself.  It will stop at
the first place you need to correct.

Some koans simply need to have the correct answer substituted for an incorrect one.
Some, however, require you to supply your own answer.  If you see the method `__` (a
double underscore) listed, it is a hint to you to supply your own code in order to
make it work correctly.

## Installing Ruby

Comming soon, you will find inside the [TangoSource Wiki](https://github.com/tangosource/wiki) 
the necessary information about how to install ruby on Linux/Unix Systems, and Mac OS X.

## The Path To Enlightenment

You can run the tests through rake or by calling the file itself (rake is the
recommended way to run them as we might build more functionality into this task).

Unix platforms, from the koans directory

    [ruby_koans] $ rake                           # runs the default target :walk_the_path
    [ruby_koans] $ ruby path_to_enlightenment.rb  # simply call the file directly
git@github.com:tangosource/wiki.git
Windows is the same thing

    c:\ruby_koans\rake                             # runs the default target :walk_the_path
    c:\ruby_koans\ruby path_to_enlightenment.rb    # simply call the file directly

### Red, Green, Refactor

In test-driven development the mantra has always been, red, green, refactor.  Write a
failing test and run it (red), make the test pass (green), then refactor it (that is
look at the code and see if you can make it any better.  In this case you will need
to run the koan and see it fail (red), make the test pass (green), then take a
moment and reflect upon the test to see what it is teaching you and improve the
code to better communicate its intent (refactor).

The very first time you run it you will see the following output:

    [ ruby_koans ] $ rake
    (in /Users/person/dev/ruby_koans)
    cd koans

    Thinking AboutAsserts
      test_assert_truth has damaged your karma.

    You have not yet reached enlightenment ...
    <false> is not true.

    Please meditate on the following code:
    ./about_asserts.rb:10:in `test_assert_truth'
    path_to_enlightenment.rb:27

    mountains are merely mountains

You have come to your first stage. If you notice it is telling you where to look for
the first solution:

    Please meditate on the following code:
    ./about_asserts.rb:10:in `test_assert_truth'
    path_to_enlightenment.rb:27

We then open up the about_asserts.rb file and look at the first test:

    # We shall contemplate truth by testing reality, via asserts.
    def test_assert_truth
      assert false                # This should be true
    end

We then change the `false` to `true` and run the test again.  After you are
done, think about what you are learning.  In this case, ignore everything except
the method name (`test_assert_truth`) and the parts inside the method (everything
before the `end`).

In this case the goal is for you to see that if you pass a value to the `assert`
method, it will either ensure it is `true` and continue on, or fail if in fact
the statement is `false`.

#### Special thanks

To [edgecase](https://github.com/edgecase) for their RubyKoans repository, you can fork it and make your own.

http://i.creativecommons.org/l/by-nc-sa/3.0/88x31.png

RubyKoans is released under a Creative Commons,
Attribution-NonCommercial-ShareAlike, Version 3.0
(http://creativecommons.org/licenses/by-nc-sa/3.0/) License.

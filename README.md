# tuneup_check_bug_repro

A repro case for [https://github.com/google/tuneup.dart/issues/32].

To repro:

* run `pub get`
* run `pub run tuneup check`.

You should see a analysis warning `The return type 'int' is not a 'String', as defined by the method 'foo'`, but it's not caught.

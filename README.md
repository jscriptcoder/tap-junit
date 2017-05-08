[![Build Status](https://travis-ci.org/dhershman1/tap-junit.svg?branch=master)](https://travis-ci.org/dhershman1/tap-junit)
# tap-junit

XML TAP output formatter for junit.

Works with tape and other tap based tests just pipe it into tap-junit and set your output param.

## Parameters

`--output` - designate where you want the .xml results to output

## Installation

~~~ text
npm install -g tap-junit
npm install tap-junit --save-dev
~~~

## Usage

~~~ text
tape test/*.js | tap-junit --output output/test
node test.js | ./node_modules/tap-junit/bin/tap-junit --output output/test
~~~

## Output

```xml
<testsuites>
  <testsuite tests="3" failures="0" errors="0" name="example tests">
    <testcase name="#1 Results should return val"/>
    <testcase name="#2 results should return newVal"/>
    <testcase name="#3 should not change param should return sameVal"/>
  </testsuite>
</testsuites>
```

## Changelog
> v1.0.3
> - Removed Tape Dependency
> - Swapped stuff over to github
> - Readme Tweaks

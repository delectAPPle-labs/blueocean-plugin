> Analytics Tools to be injected in to BlueOcean UI

# RollBar

* Enable RollBar

RollBar is disabled by default. Use BLUEOCEAN_ROLLBAR_ENABLED JVM property to enable.

```` 
mvn hpi:run -DBLUEOCEAN_ROLLBAR_ENABLED=true
```` 


## Usage ...

    try {
        foo();
        $blueocean_Rollbar.debug('foo() called');
    } catch (e) {
        $blueocean_Rollbar.error('Problem calling foo()', e);
    }

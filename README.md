## angular-delay-register

Add additional methods to Angular Module so that we can register controllers/directives/services/factories after bootstrap

#### Set Up

```
var module = angular.module( 'myApp', [] );
var delay = require( 'angular-delay-register' );

module = delay.configureApp( module );

module.run([ '$couchPotato', function( $couchPotato ){
    module.lazy = $couchPotato; //note that you need to use the name 'lazy'
}]);
```
#### History/Attribution

angular-delay-register is modified from [angular-couch-potato](https://github.com/laurelnaiad/angular-couch-potato).

#### License

See the [LICENSE file](https://github.com/neekey/angular-delay-register/blob/master/LICENSE).

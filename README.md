findings:
 - initial investigation: https://github.com/ef4/ember-auto-import/issues/564#issuecomment-1426931012
 - importing RSVP in the app gives:
   ```
   TypeError: RSVP.configure is not a function
   ```
 - empty early bootset = no error
 - testing individual entries from the default earlyBootSet.
   all of these are commented out in the ember-cli-build.js
    - only `@glimmer/component` error
    - only `@glimmer/tracking` - no error
    - only `@ember/service` - error
    - only `@ember/controller` - error
    - only `@ember/component` - error
    - only `@ember/routing/route` - error

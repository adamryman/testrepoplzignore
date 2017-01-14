# GOVENDOR TEST PLZ IGNORE

I'm trying to increase the speed of `govendor sync` by having it use the cache
if it can before trying to update the cache. If that does not work update the
cache and try again.

The repo will be pushed with commit `766da4a9918ca6755a7e9730f741ae97da65033a`.

Then I will use govendor to fetch/sync it to another project.

I will then commit on this package repo again, push it, and then update the
`sha` in the vendor/vendor.json file by hand.

I will then run `govendor sync` and see how it handles the commit not exising in
the cache with the changes I made. I hope it will pull the changes and then
chage to the correct revision. We will see.

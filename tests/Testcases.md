
Test cases
==========

Summary
-------

* Upload a new file, share it (this will affect the time stamp): Recalculate
  the local files checksum and compare it with upstream.  If equal only update
  the time stamp.
* Empty configuration. Expected result: OneDrive should not start up
* User A and B synchronize; While working with the same directory user A deletes the directory (or moves it outside the selective sync area), user B modifies a file in the directory. Expected Result: ?
* File upload should resume (not restart) - if that is possible.
* Don't leave incomplete files in the filesystem when space runs out - either
  don't download or delete the file when it turns out there's not enough space

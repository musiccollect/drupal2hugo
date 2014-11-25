# Drupal2Hugo

Drupal2Hugo provides a basic converter to export a Drupal website to text files in Hugo format. It will do a lot of
the work for you, but some manual intervention will still be needed.

* For each Drupal node, a corresponding text file is written containing the metadata (front matter)
  and the node body content.

* If the Drupal node has a summary, it is retained as a comment after the front matter. It will require
  manual editing to mark the body so that the summary produced by Hugo matches that in Drupal.

* The Drupal markup is assumed to be Markdown or (a subset of) HTML. The body content is transferred verbatim
  and will only work properly if Markdown or HTML have been used.

* All other Drupal content fields are lost. In particular, note that pictures and other multimedia content
  need to be dealt with manually, although the links to them in the body content will be retained.

This is experimental. YMMV.

MIT Licence.

[![Build Status](https://drone.io/bitbucket.org/rickb777/drupal2hugo/status.png)](https://drone.io/bitbucket.org/rickb777/drupal2hugo/latest)

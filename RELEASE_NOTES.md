# Release Notes

## XMLUnit for Java 2.0.0-alpha-04

* the `schemaURI` in `Validator` has been pushed down to
  `ParsingValidator` since it is only used inside this class.
* the mapping of `DifferenceEngine#setNamespaceContext` has been
  inverted from prefix -> URI to URI -> prefix in order to be
  consistent with the same concept in `XPathEngine`.
* `CommentLessSource` uses an XSLT stylesheet internally which lacked
  the required `version` attribute. PR
  [#47](https://github.com/xmlunit/xmlunit/pull/47) by
  [@phbenisc](https://github.com/phbenisc).

## XMLUnit for Java 2.0.0-alpha-03 - /Released 2015-12-13/

* the xmlunit-parent POM no longer uses the deprecated
  `org.sonatype.oss:oss-parent` as its parent.
* added new overloads to `XPathEngine`
* fixed the XPath context used by the `byXPath` element selector so
  that "." now refers to the current element.
  Issue [#39](https://github.com/xmlunit/xmlunit/issues/39)
* `ElementSelectors#conditionalBuilder` now stops at the first
  predicate returning `true`, even if the associated `ElementSelector`
  returns false.
  Issue [#40](https://github.com/xmlunit/xmlunit/issues/40)

## XMLUnit for Java 2.0.0-alpha-02 - /Released 2015-11-21/

This is the initial alpha release of XMLUnit.NET.  We expect the API
to change for the next release based on user feedback.

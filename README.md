## TODO

- Add component-level documentation and tests for dplmrts_invocablearchetype
  and update dplmrts's documentation.
- Add component-level documentation and tests for dplp's components
  and update dplp's documentation.
  - dplp_anypromise
  - dplp_promise
  - dplp_resolver (perhaps we want a dplp_resolverachtype to help unit test
    dplp_promise)
- Look at the documentation for the FindGTest CMake module and use that as a
  starting point for discovering how to better integrate the unit tests. Once
  we get a way to run the unit tests we should describe how in `dpl`s readme.
- Add documentation of system error exceptions to apltcp_channel.
- Add documentation for "ArchType".
- Add documentation for dplm17_variant.
- Fix the included guards. INCLUDED should be coming first.
- Consider a generalization of `dplmrts::AnyTuple` which is satisified when an
  arbitrary template class is matched.
- Add to (new?) standard.
  - "This concept is satisfied by"
  - Markdown formatting for README's, etc.
- Figure out if we need a "Package Synopsis" *and* a "Package Overview" when
  documenting package groups.
- Make cmsfm_findasio more robust when it cannot find the 'asio' directory.

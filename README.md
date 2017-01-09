# superpromise

**PURPOSE:** Provide a super project for promise related groups

## Description

The `superpromise` superproject contains groups related to promises. The intent
is to provide a convenient way to develop promises and groups frequently
modified in tandem with them.

## TODO

- Add component-level documentation and tests for dplp's components and update
  dplp's documentation.
  - dplp_promisestateimp
  - dplp_promisestateimputil
  - dplp_promisestate
  - dplp_promise (perhaps we want a dplp_resolverachtype to help unit test
    dplp_promise)
- Add documentation of system error exceptions to apltcp_channel.
- Add documentation for dplm17_variant.
- Consider a generalization of `dplmrts::AnyTuple` which is satisified when an
  arbitrary template class is matched.
- Add to (new?) standard.
  - "This concept is satisfied by"
  - Markdown formatting for README's, etc.
- Figure out if we need a "Package Synopsis" *and* a "Package Overview" when
  documenting package groups.
- Make cmsfm_findasio more robust when it cannot find the 'asio' directory.
- Narrow down the dplp_resolver problem and write an email to Andrew Sutton
  asking what's up with this case.

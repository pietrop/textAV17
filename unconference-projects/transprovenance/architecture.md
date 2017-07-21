# Data pipeline
1. Input: target web URL (the edited video)

2. Processing:
  * Request metadata from an external source (e.g. Internet Archive)
    * source locations (e.g. URLs)
    * time (start and end of source, start and end of target URL)
    * other extra information (filmed by, title etc.)
    * captions metadata
  * Render - Have an chimera HLS manifest file from the data
    * make rendering fast
3. Output:
  * Captions
  * Video


# Data model

# Users needs
Not considered
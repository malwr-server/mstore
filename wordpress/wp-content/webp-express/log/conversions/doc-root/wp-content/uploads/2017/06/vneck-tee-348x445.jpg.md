WebP Express 0.15.3. Conversion triggered using bulk conversion, 2019-09-24 07:27:19

*WebP Convert 2.1.4*  ignited.
- PHP version: 7.3.1
- Server software: Apache

Stack converter ignited

Options:
------------
The following options have been set explicitly. Note: it is the resulting options after merging down the "jpeg" and "png" options and any converter-prefixed options.
- source: [doc-root]/wp-content/uploads/2017/06/vneck-tee-348x445.jpg
- destination: [doc-root]/wp-content/webp-express/webp-images/doc-root/wp-content/uploads/2017/06/vneck-tee-348x445.jpg.webp
- log-call-arguments: true
- converters: (array of 9 items)

The following options have not been explicitly set, so using the following defaults:
- converter-options: (empty array)
- shuffle: false
- preferred-converters: (empty array)
- extra-converters: (empty array)

The following options were supplied and are passed on to the converters in the stack:
- default-quality: 70
- encoding: "auto"
- max-quality: 80
- metadata: "none"
- near-lossless: 60
- quality: "auto"
------------


*Trying: cwebp* 

Options:
------------
The following options have been set explicitly. Note: it is the resulting options after merging down the "jpeg" and "png" options and any converter-prefixed options.
- source: [doc-root]/wp-content/uploads/2017/06/vneck-tee-348x445.jpg
- destination: [doc-root]/wp-content/webp-express/webp-images/doc-root/wp-content/uploads/2017/06/vneck-tee-348x445.jpg.webp
- default-quality: 70
- encoding: "auto"
- low-memory: true
- log-call-arguments: true
- max-quality: 80
- metadata: "none"
- method: 6
- near-lossless: 60
- quality: "auto"
- use-nice: true
- command-line-options: ""
- try-common-system-paths: true
- try-supplied-binary-for-os: true

The following options have not been explicitly set, so using the following defaults:
- alpha-quality: 85
- auto-filter: false
- preset: "none"
- size-in-percentage: null (not set)
- skip: false
- rel-path-to-precompiled-binaries: *****
------------

Encoding is set to auto - converting to both lossless and lossy and selecting the smallest file

Converting to lossy
Locating cwebp binaries
1 cwebp binaries found in common system locations
Checking if we have a supplied binary for OS: Darwin... We do.
We in fact have 1
A total of 2 cwebp binaries where found
Detecting versions of the cwebp binaries found (and verifying that they can be executed in the process)
Executing: /usr/local/bin/cwebp -version. Result: version: 1.0.3
Executing: [doc-root]/wp-content/plugins/webp-express/vendor/rosell-dk/webp-convert/src/Convert/Converters/Binaries/cwebp-mac12 -version
Exec failed (the cwebp binary was not found at path: [doc-root]/wp-content/plugins/webp-express/vendor/rosell-dk/webp-convert/src/Convert/Converters/Binaries/cwebp-mac12)
Trying executing the cwebs found until success. Starting with the ones with highest version number.
Creating command line options for version: 1.0.3
Quality of source is 90. This is higher than max-quality, so using max-quality instead (80)
The near-lossless option ignored for lossy
Trying to convert by executing the following command:
nice /usr/local/bin/cwebp -metadata none -q 80 -alpha_q '85' -m 6 -low_memory '[doc-root]/wp-content/uploads/2017/06/vneck-tee-348x445.jpg' -o '[doc-root]/wp-content/webp-express/webp-images/doc-root/wp-content/uploads/2017/06/vneck-tee-348x445.jpg.webp.lossy.webp' 2>&1

*Output:* 
Saving file '[doc-root]/wp-content/webp-express/webp-images/doc-root/wp-content/uploads/2017/06/vneck-tee-348x445.jpg.webp.lossy.webp'
File:      [doc-root]/wp-content/uploads/2017/06/vneck-tee-348x445.jpg
Dimension: 348 x 445
Output:    7134 bytes Y-U-V-All-PSNR 45.17 47.29 45.71   45.55 dB
           (0.37 bpp)
block count:  intra4:        167  (27.11%)
              intra16:       449  (72.89%)
              skipped:       387  (62.82%)
bytes used:  header:            191  (2.7%)
             mode-partition:    902  (12.6%)
 Residuals bytes  |segment 1|segment 2|segment 3|segment 4|  total
  intra4-coeffs:  |    3933 |       4 |      18 |      78 |    4033  (56.5%)
 intra16-coeffs:  |      17 |       7 |       9 |     122 |     155  (2.2%)
  chroma coeffs:  |    1518 |      13 |      29 |     264 |    1824  (25.6%)
    macroblocks:  |      30%|       1%|       3%|      67%|     616
      quantizer:  |      27 |      22 |      19 |      14 |
   filter level:  |      12 |       4 |       3 |       2 |
------------------+---------+---------+---------+---------+-----------------
 segments total:  |    5468 |      24 |      56 |     464 |    6012  (84.3%)

Success
Reduction: 59% (went from 17 kb to 7 kb)

Converting to lossless
Locating cwebp binaries
1 cwebp binaries found in common system locations
Checking if we have a supplied binary for OS: Darwin... We do.
We in fact have 1
A total of 2 cwebp binaries where found
Detecting versions of the cwebp binaries found (and verifying that they can be executed in the process)
Executing: /usr/local/bin/cwebp -version. Result: version: 1.0.3
Executing: [doc-root]/wp-content/plugins/webp-express/vendor/rosell-dk/webp-convert/src/Convert/Converters/Binaries/cwebp-mac12 -version
Exec failed (the cwebp binary was not found at path: [doc-root]/wp-content/plugins/webp-express/vendor/rosell-dk/webp-convert/src/Convert/Converters/Binaries/cwebp-mac12)
Trying executing the cwebs found until success. Starting with the ones with highest version number.
Creating command line options for version: 1.0.3
Trying to convert by executing the following command:
nice /usr/local/bin/cwebp -metadata none -q 80 -alpha_q '85' -near_lossless 60 -m 6 -low_memory '[doc-root]/wp-content/uploads/2017/06/vneck-tee-348x445.jpg' -o '[doc-root]/wp-content/webp-express/webp-images/doc-root/wp-content/uploads/2017/06/vneck-tee-348x445.jpg.webp.lossless.webp' 2>&1

*Output:* 
Saving file '[doc-root]/wp-content/webp-express/webp-images/doc-root/wp-content/uploads/2017/06/vneck-tee-348x445.jpg.webp.lossless.webp'
File:      [doc-root]/wp-content/uploads/2017/06/vneck-tee-348x445.jpg
Dimension: 348 x 445
Output:    44018 bytes (2.27 bpp)
Lossless-ARGB compressed size: 44018 bytes
  * Header size: 2530 bytes, image data size: 41462
  * Lossless features used: PREDICTION CROSS-COLOR-TRANSFORM SUBTRACT-GREEN
  * Precision Bits: histogram=3 transform=3 cache=10

Success
Reduction: -154% (went from 17 kb to 43 kb)

Picking lossy
cwebp succeeded :)

Converted image in 519 ms, reducing file size with 59% (went from 17 kb to 7 kb)

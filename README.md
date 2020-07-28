# abeeway_ttn_decoder

This is a simple payload decoder example for some of Abeeway's LoRaWAN asset tracking devices.

It has been tested with the Micro Tracker only at this point.

It is designed for use with TheThingsNetwork but can easily be adapted for use with Chirpstack (instructions to follow).

**Note:** this is designed for testing purposes only, I take no responsibility for anyone using this getting missing or incorrect data!

## The Things Network Instructions

Simply copy and paste the code from decoder.js into the Payload Formats tab in your TTN application. Into the decoder box, replacing anything already in there.

## Chirpstack Instructions

1. Create a device profile for Abeeway Asset Trackers if you don't already have one.
1. In the codec tab, select "Custom JavaScript codec functions".
1. Copy and paste the code from decoder.js into the upper text box, replacing anything that was already in there.
1. Change the "Decoder" function name to "Decode".
1. Swap this function's parameters around. So instead of "(bytes, fport)" you have "(fport, bytes)".

Paul Hayes - paul@alliot.co.uk
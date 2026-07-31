# gndless_midi

MIDIのbyte receiverのRTL実装です。
baud rateを31,250に固定したuartです。

MIDI message parserではありません。
適宜ソフトコアCPUなどでparseしてください。

```veryl
inst midi: midi::MidiRx #( CLOCK_HZ: 50_000_000 ) (...);
```

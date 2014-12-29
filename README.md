# Eaglesong

## About

Eaglesong is a fast replay parser for Dota2, written in .NET

## Usage

As of version 0.1, you can use Eaglesong by referencing the dll and get the list of messages:
```C#
LinkedList<object> messages = Eaglesong.DemParser.Read("path-to-replay.dem");
```

## Runtime

#####V0.1
- 1 hour match, 58,923 messages: 00m 00s 984ms

## Protobuf Data

The protobuf data used is from [skadistats's smoke](https://github.com/skadistats/smoke/), which in turn is from [SteamKitRE](https://github.com/SteamRE/SteamKit).  
Big thanks to the guys at skadistats for their [helpful guide on the makeup of a Dota2 replay](https://github.com/skadistats/smoke/wiki/Anatomy-of-a-Dota-2-Replay-File)!

## Libraries

Eaglesong requires the following libraries:
- [protobuf-net](https://github.com/mgravell/protobuf-net)
- [Snappy.NET (and subsequently Crc32C.NET)](http://snappy.angeloflogic.com/)
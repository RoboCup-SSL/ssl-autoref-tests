# Testcases for the RoboCup SSL automatic referees
For every rule checked by the automatic referees (see the [official ssl rules](https://robocup-ssl.github.io/ssl-rules/sslrules.html) for details),
there is one folder containing both positive and negative tests for that rule.

Every test consists of one log file (see https://ssl.robocup.org/game-logs/ for the format description) and one JSON file encoding a protobuf
packet describing the desired event in the log file.
They are matched by the file name, differing only in the ending (.log vs .json).
The JSON files contain a JSON serialized version of a DesiredEvent packet as described in [desired_event_description.proto](desired_event_description.proto).

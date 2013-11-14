FileAPI.lineReader
==================

A line reader for the browser that supports large files.


Example
-------

    readLines(file, function (line, lineNumber, callback) {
        console.log("Ready to do something with line", lineNumber);
        callback();
    }, function (err) {
        if (err !== null) {
            console.error("An error occured:", err);
        } else {
            console.log("Done reading file.");
        }
    });

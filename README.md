#### usage
scheduleTask(time, callback);
Examples
Execute a task every 1 second:

javascript
Copy code
scheduleTask('1s', () => console.log('Task executed every 1 second.'));
Execute a task every 3 minutes:

javascript
Copy code
scheduleTask('3m', () => console.log('Task executed every 3 minutes.'));
Execute a task every 2 hours:

javascript
Copy code
scheduleTask('2h', () => console.log('Task executed every 2 hours.'));
Execute a task every day at 8 AM:

javascript
Copy code
scheduleTask('d8', () => console.log('Task executed every day at 8 AM.'));
Execute a task every day at 3 AM:

javascript
Copy code
scheduleTask('d3', () => console.log('Task executed every day at 3 AM.'));
Time Units and Range of Values
s (seconds): 1 to 59
m (minutes): 1 to 59
h (hours): 1 to 24
d (daily): 0 to 23 (where 0 represents midnight, 12 AM)
Notes
For daily occurrences ('d'), the hour value should be specified in the range 0 to 23.

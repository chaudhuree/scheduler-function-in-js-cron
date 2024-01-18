## Usage

### Function Signature

```javascript
scheduleTask(time, callback);
```

### Parameters

* `time` (String): A string representing the time interval or schedule. Examples: '1s' (1 second), '3m' (3 minutes), '2h' (2 hours), 'd8' (every day at 8 AM).
* `callback` (Function): The function to be executed at the specified time or interval.

### Examples

1. Execute a task every 1 second:
    
    ```javascript
    scheduleTask('1s', () => console.log('Task executed every 1 second.'));
    ```
    
2. Execute a task every 3 minutes:
    
    ```javascript
    scheduleTask('3m', () => console.log('Task executed every 3 minutes.'));
    ```
    
3. Execute a task every 2 hours:
    
    ```javascript
    scheduleTask('2h', () => console.log('Task executed every 2 hours.'));
    ```
    
4. Execute a task every day at 8 AM:
    
    ```javascript
    scheduleTask('d8', () => console.log('Task executed every day at 8 AM.'));
    ```
    
5. Execute a task every day at 3 AM:
    
    ```javascript
    scheduleTask('d3', () => console.log('Task executed every day at 3 AM.'));
    ```
    

### Time Units

* `s`: seconds: 1 to 59
* `m`: minutes: 1 to 59
* `h`: hours: 1 to 24
* `d`: daily: 0 to 23 (where 0 represents midnight, 12 AM)

### Notes

* For daily occurrences ('d'), the hour value should be specified in the range 0 to 23.

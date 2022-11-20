# learn-aspnetcore

Learn to create a web API with ASP.NET Core based [this tutorial](https://learn.microsoft.com/en-us/aspnet/core/tutorials/first-web-api?view=aspnetcore-7.0&tabs=visual-studio-code).

## Test Run Locally

1. <kbd>Ctrl</kbd> + <kbd>F5</kbd> or go to Menu -> Run -> Run Without Debugging
2. The browser should be automatically opened. Otherwise, grab the server URL and post from the debug console log.
3. Open Swagger page at path `/swagger`.
4. You can test <kbd>GET</kbd> `/WeatherForcast` API on the Swagger page and you should see response similar to this:

```json
[
  {
    "date": "2022-11-21T14:45:12.162479+07:00",
    "temperatureC": 14,
    "temperatureF": 57,
    "summary": "Warm"
  },
  {
    "date": "2022-11-22T14:45:12.162841+07:00",
    "temperatureC": 1,
    "temperatureF": 33,
    "summary": "Cool"
  },
  {
    "date": "2022-11-23T14:45:12.162849+07:00",
    "temperatureC": -19,
    "temperatureF": -2,
    "summary": "Sweltering"
  },
  {
    "date": "2022-11-24T14:45:12.16285+07:00",
    "temperatureC": 21,
    "temperatureF": 69,
    "summary": "Balmy"
  },
  {
    "date": "2022-11-25T14:45:12.16285+07:00",
    "temperatureC": 10,
    "temperatureF": 49,
    "summary": "Freezing"
  }
]
```

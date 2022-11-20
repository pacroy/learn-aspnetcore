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
    "date": "2022-11-21",
    "temperatureC": 27,
    "temperatureF": 80,
    "summary": "Balmy"
  },
  {
    "date": "2022-11-22",
    "temperatureC": -13,
    "temperatureF": 9,
    "summary": "Cool"
  },
  {
    "date": "2022-11-23",
    "temperatureC": -15,
    "temperatureF": 6,
    "summary": "Freezing"
  },
  {
    "date": "2022-11-24",
    "temperatureC": 25,
    "temperatureF": 76,
    "summary": "Mild"
  },
  {
    "date": "2022-11-25",
    "temperatureC": 41,
    "temperatureF": 105,
    "summary": "Bracing"
  }
]
```

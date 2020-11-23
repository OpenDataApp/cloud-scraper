# Oracle provider

The purpose of this repo is create a mechanism to get cloud docs, text, images, etc, from Oracle cloud provider. To do that, our approach was to use web crawwlers to extract data from different sources:

- [Oracle Architecture Center](https://docs.oracle.com/en/solutions/index.html)

## Scrappers

- **Approach 1 - [example](./1-bs4):** use `python` libraries as `bs4` and `Soup and Request`, this way is simple and powerful, but, Isn't posible deal with `javascript(js)` escenarios.

- **Approach 2 - [example](./2-selenium):** to deal with `js` the option was to use `selenium` with `firefox` and `geckodriver`.

## Disclaimer

The views expressed on this repository are my own and do not reflect the views of the company(ies) I work (or have worked for) neither Oracle Corporation. The opinions expressed by visitors on this repository are theirs, not mine.

The information in this repository is written based on personal experiences. You are free to use the information on this repository but I am not responsible and will not compensate to you if you ever happen to suffer a loss/inconvenience/damage because of/while making use of this information.
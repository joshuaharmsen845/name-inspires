# Verbs

This part is consists of verbs that are going to be used as part of the naming convention. verbs are recommended to be used for a function that is going to perform a command.

**Columns guide** :

- Name : The name of the verb
- Guess Functionality: What a third party reader will guess about the code with that name about the functionality without reading it. This part is not very accurate but tries to give some sense.
- Guess Return Type: What a third party may think about the return type of the method or variable without checking that. This part is not very accurate but tries to give some sense.
- Examples: Consist of real use-case examples that help you to understand the use-cases better.
- Bad Usage: Misuse that another third party may make a mistake while reading as examples.

| Name     | Guess Functionality                                                                                         | Guess Return Type                                                                                                                                          | Good Naming Examples                                                                                   | Bad Naming Examples                                                 |
| -------- | ----------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------- |
| Get      | fetch resource as expected in a suitable form for the specific part of the execution                        | Fully prepared data if exists **OTHERWISE** throws an exception if it should exist but doesn't                                                             | GetResponse, GetUserEmail, GetDatabaseConnection, GetSanitizedString, GetQueryLog, GetHttp, GetContext | NEED CONTRIBUTION                                                   |
| Set      | Store (or config) specific resource                                                                         | Boolean indicates that resource was stored correctly or not **OTHERWISE** Throw an exception in case of misbehaving.                                       | SetBackOfJitterConnection, SetSession, SetFilter, SetFirstNameAttribute                                | SetData: It does not indicate what kind of data is going to be set. |
| Unset    | Returns the source to its initial state. The initial state can also indicate the destruction of the source. | The source before it deletion **OR** a boolean indicates the resource was unset or not. **OTHERWISE** an exception will be raised if misbehaving accuered. | UnsetCardNumber, UnsetBearerToken, UnsetApiThrottlingCounter, UnsetProxyWatcher, UnsetCookies          | _NEED CONTRIBUTION_                                                 |
| **Name** | **Guess Functionality**                                                                                     | **Guess Return Type**                                                                                                                                      | **Good Naming Examples**                                                                               | **Bad Naming Example**                                              |

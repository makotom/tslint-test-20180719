This is a showcase that very-long functions may be accepted by max-func-body-length rule if the function is defined as a parameter of a pre-defined function/method, of which name matches `/^.*describe.*$/`.

Just `npm i` and `npm lint` for your try.

[The behaviour could be an expected one](https://github.com/Microsoft/tslint-microsoft-contrib/blob/master/src/maxFuncBodyLengthRule.ts#L25), but the pattern mathces to names which do not look like `describe`, such as `xyzdescribexyz` for example, this is not a good idea.

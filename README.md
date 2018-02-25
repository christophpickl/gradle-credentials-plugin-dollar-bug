# gradle-credentials-plugin-dollar-bug

This repo simply reproduces the bug issued here: https://github.com/etiennestuder/gradle-credentials-plugin/issues/18

## Howto

First add an encrypted value:

	$ gradle addCredentials --key dollarKey --value before$after

 Then print that value

 	$ gradle printDollarValue

This will print `dollar value: 'before'` instead of the expectd `dollar value: 'before$after'`

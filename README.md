=ЗНАЧЕН(REGEXREPLACE(REGEXEXTRACT(IMPORTXML("https://etherscan.io/address/"&box with your address&"";"//*[text()='Value:']/following-sibling::div/text()");"\d\.?\d+"); "^(\d+)(?:[.,](\d*).*)?"; "$1,$2\0"))
=ЗНАЧЕН(REGEXREPLACE(REGEXEXTRACT(IMPORTXML("https://etherscan.io/address/"&box with your address&"";"//div[@class='position-relative w-100 mr-1']/a");"\d\.?\d+"); "^(\d+)(?:[.,](\d*).*)?"; "$1,$2\0"))
The first script shows the amount of native token.
The second is the total value of tokens in the wallet

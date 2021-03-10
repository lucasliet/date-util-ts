# Date Util
Date handler to parse string and date in ISO and BR format

## installation
```SH
yarn add @lucasliet/date-util
```

## usage

```TS
import DateUtil from '@lucasliet/date-util';

const dateBR: string = DateUtil.toBRFormat(new Date());   //returns string in dd/MM/yyyy format

const dateISO: string = DateUtil.toISOFormat(dateBR);     //returns string in yyyy-MM-yyyy format

const isBRFormat: boolean = DateUtil.isBRFormat(dateBR);  //check if string pattern matches dd/MM/yyyy format

const date: Date = DateUtil.parseDate(dateBR);            //returns a date Object from dd/MM/yyyy or yyyy-MM-dd string format
```
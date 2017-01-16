# nbastats

'link to NBA player rater'

https://docs.google.com/spreadsheets/d/1iSIrNw4Kf9ikw3eEGIUUcuO3EK-17qqiPuQ99ftqSiE/edit?usp=sharing

'to update the data'

function getData() {
  var queryString = Math.random();
  var cellFunction = '=IMPORTHTML("http://www.basketball-reference.com/leagues/NBA_2017_per_game.html?' + queryString + '","table",1)';

  SpreadsheetApp.getActiveSheet().getRange('A1').setValue(cellFunction);
}

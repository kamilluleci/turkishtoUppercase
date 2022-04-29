# turkishtoUppercase
Turkish char to upper


  turkishToUpper(tmpStr: string): string {
    var string = tmpStr;
    var letters = { i: "İ", ş: "Ş", ğ: "Ğ", ü: "Ü", ö: "Ö", ç: "Ç", ı: "I" };
    string = string.replace(/(([iışğüçö]))/g, function (letter) {
      return letters[letter];
    });
    return string.toUpperCase();
  }

        $scope.getDigitBanglaFromEnglish = function (EnglishNumber) {
           var finalEnlishToBanglaNumber = { '0': '০', '1': '১', '2': '২', '3': '৩', '4': '৪', '5': '৫', '6': '৬', '7': '৭', '8': '৮', '9': '৯' };
            for (var x in finalEnlishToBanglaNumber) {
                EnglishNumber = EnglishNumber.replace(new RegExp(x, 'g'), finalEnlishToBanglaNumber[x]);
            }
            return EnglishNumber;
        };
        console.log($scope.getDigitBanglaFromEnglish('12345'));

        $scope.getDigitBanglaFromEnglish = function (Number) {
           var finalEnlishToBanglaNumber = { '0': '০', '1': '১', '2': '২', '3': '৩', '4': '৪', '5': '৫', '6': '৬', '7': '৭', '8': '৮', '9': '৯' };
            for (var x in finalEnlishToBanglaNumber) {
                Number = Number.replace(new RegExp(x, 'g'), finalEnlishToBanglaNumber[x]);
            }
            return Number;
        };
        console.log($scope.getDigitBanglaFromEnglish('12345'));

# Markdown & Git

# Raman Krutsiou

# Contacts:

  - Phone: + 375 (33) 647 92 45
  - Email:  krutev2016@mail.ru 


# Summary
  Currently, I work as an engineer in the field of mechanical engineering. However, mechanical engineering is in decline, so I decided to change my profession.The Rolling Scopes School gives me the opportunity to learn a new, very interesting profession.
  
# Skills
- C;
- Objective-C;
- Xcode.

# Code examples
```
NSString* const GovermentTaxLevelDidChangeNotificdtion =@"GovermentTaxLevelDidChangeNotificdtion";
NSString* const GovermentSalaryChangeNotificdtion =@"GovermentSalaryChangeNotificdtion";
NSString* const GovermentPensionlDidChangeNotificdtion = @"GovermentPensionlDidChangeNotificdtion";
NSString* const GovermentAveregePriceDidChangeNotificdtion =@"GovermentAveregePriceDidChangeNotificdtion" ;

NSString* const GovermentTaxLevelUserInfoKey = @"GovermentTaxLevelUserInfoKey";
NSString* const GovermentSalaryUserInfoKey = @"GovermentSalaryUserInfoKey";
NSString* const GovermentPensionlUserInfoKey = @"GovermentPensionlUserInfoKey";
NSString* const GovermentAveregePriceUserInfoKey = @"GovermentAveregePriceUserInfoKey";

@implementation Government
- (id) init{
    self = [super init];
    if (self) {
        _taxLevel =5.f;
        _salary = 1000;
        _pension = 500;
        _averagePrice = 10;
    }
    return self;
}

-(void) setTaxLevel:(float)taxLevel{
    _taxLevel = taxLevel;
    
    NSDictionary* dictionary  = [NSDictionary dictionaryWithObject:[NSNumber numberWithFloat:taxLevel] forKey:GovermentTaxLevelUserInfoKey];
    
    [[NSNotificationCenter defaultCenter] postNotificationName:GovermentTaxLevelDidChangeNotificdtion object:nil userInfo:dictionary];
}

- (void)setSalary:(float)salary {
    _salary = salary;
    NSDictionary* dictionary  = [NSDictionary dictionaryWithObject:[NSNumber numberWithFloat:salary] forKey:GovermentSalaryUserInfoKey];
 
    [[NSNotificationCenter defaultCenter]postNotificationName:GovermentSalaryChangeNotificdtion object:nil userInfo:dictionary];
    
}

-(void)setPension:(float)pension {
    _pension = pension;
    NSDictionary* dictionary = [NSDictionary dictionaryWithObject:[NSNumber numberWithFloat:pension] forKey:GovermentPensionlUserInfoKey];
    [[NSNotificationCenter defaultCenter]postNotificationName:GovermentPensionlDidChangeNotificdtion object:nil userInfo:dictionary];
    
}


-(void)setAveragePrice:(float)averagePrice{
    _averagePrice = averagePrice;
    NSDictionary* dictionary = [NSDictionary dictionaryWithObject:[NSNumber numberWithFloat:averagePrice] forKey:GovermentAveregePriceUserInfoKey];
    [[NSNotificationCenter defaultCenter] postNotificationName:GovermentAveregePriceDidChangeNotificdtion object:nil userInfo:dictionary];
}
@end
```
# Education
-BNTU 2019 (Mechanical Engineering Technology)
# Courses:

-iOS Development

# English level
Intermediate

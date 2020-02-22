# Iaroslav Denisenko

## Contact Info:

* Phone: +7(495) 123-45-67
* E-mail: yaroslav1985@gmail.com
* VK: https://vk.com/yaroslavdenisenko

## About me

I have been working in technical support for about 10 years. Time passes ... I am almost 35 years old. Despite the fact that I have a leading position, I have no prospects for further development. Therefore, I decided to develop in the direction of developing software for mobile devices on iOS. I have a little programming experience in C, Objective-C and Python. I hope I succeed and become a cool programmer.

## Skills

* C
* Objective-C
* Python
* XCode
* Git
* Linux
* Bash
* 1C

## Code examples

```
- (void)generateSectionsInBackkgroundFromArray:(NSArray *)array withFilter:(NSString *)filter {
    
    [self.currentOperation cancel];
    __weak ViewController *weakSelf = self;
    self.currentOperation = [NSBlockOperation blockOperationWithBlock:^{
        NSArray *sectionsArray = [weakSelf sectionsFromArray:array withFilter:filter];
        
        dispatch_async(dispatch_get_main_queue(), ^{
            
            weakSelf.sections = sectionsArray;
            [weakSelf.tableView reloadData];
            self.currentOperation = nil;
        });
    }];
    [self.currentOperation start];
}
```

## Education

Bachelor of Chemistry, 
MIREA - Russian Technological University

## English

* A2 

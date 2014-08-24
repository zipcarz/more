more
====
// Code generated with JSON Designer http://itunes.apple.com/app/json-designer/id432736126?mt=8
 
id root = @{
    @"http://www.mobilesocksproxy.com/m/getproxy/d853c443c5eea89cfa165e50ba5aa85f.pac" : @[ @{
    }]
};
 
 
NSString* url = @"your uri";
NSMutableURLRequest *request = [[NSMutableURLRequest alloc] init];
[request setURL:[NSURL URLWithString:url]];
request.HTTPMethod = @"POST";
request.HTTPBody = [NSJSONSerialization dataWithJSONObject:root options:0 error:NULL];;
     
NSError *error = nil;
NSURLResponse *resp = nil;
NSData *responseData = [NSURLConnection sendSynchronousRequest:request returningResponse:&resp error:&error];

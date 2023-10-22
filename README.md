#ifndef __OPTIMIZE__
  #import "RRFPSBar.h"
#endif

@implementation YourAppDelegate

- (BOOL)application:(UIApplication *)application didFinishLaunchingWithOptions:(NSDictionary *)launchOptions {
  // Show only if app is is not optimized (aka debug build)
#ifndef __OPTIMIZE__
    [[RRFPSBar sharedInstance] setHidden:NO];
#endif

}

@end


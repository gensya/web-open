# web-open

import UIKit

import SafariServices

class ViewController: UIViewController {

    @IBAction func tapBtn() {
        
        if let url = NSURL(string: "http://kyushu.seikyou.ne.jp/ryudai-coop/dinning/index.html"){
            
            let vc = SFSafariViewController(URL:url,entersReaderIfAvailable: true)
            
            presentViewController(vc, animated: true, completion: nil)
        }
    }
    
    func safariViewControllerDidFinish(controller: SFSafariViewController){
    }
    
    override func viewDidLoad() {
        super.viewDidLoad()
        // Do any additional setup after loading the view, typically from a nib.
    }

    override func didReceiveMemoryWarning() {
        super.didReceiveMemoryWarning()
        // Dispose of any resources that can be recreated.
    }


}

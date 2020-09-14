//
//  ViewController.swift
//  Application1
//
//  Created by Lionel Castelino on 17/08/20.
//  Copyright © 2020 CleverTap. All rights reserved.
//

import UIKit
import CleverTapSDK

class ViewController: UIViewController {
    
    @IBOutlet weak var name: UITextField!
    
    @IBOutlet weak var identity: UITextField!
    
    @IBOutlet weak var email: UITextField!
    
    @IBOutlet weak var address: UITextField!
    
    @IBOutlet weak var phone: UITextField!
    
    @IBOutlet weak var gender: UITextField!
    
    @IBOutlet weak var email_push: UITextField!
    
    @IBAction func buttonPressed3(_ sender: UIButton) {
        CleverTap.sharedInstance()?.recordEvent("Charged")
    }
    @IBAction func buttonPressed2(_ sender: UIButton) {
        CleverTap.sharedInstance()?.recordEvent("Added to Cart")
    }
    @IBAction func buttonPressed1(_ sender: Any) {
        let update: Dictionary<String, String?> = [
            
            "Email": email_push.text,
            
            ]
        
        CleverTap.sharedInstance()?.profilePush(update as [AnyHashable:Any]);
    }
    @IBAction func buttonPressed(_ sender: Any) {
        let login: Dictionary<String, String?> = [
            "Name": name.text,
            "Identity": identity.text,
            "Email": email.text,
            "Location": address.text,
            "Phone No.": phone.text,
            "Gender": gender.text,
            
            ]
        
        CleverTap.sharedInstance()?.onUserLogin(login as [AnyHashable:Any]);
    }
    override func viewDidLoad() {
        super.viewDidLoad()
        /*let login: Dictionary<String, String> = [
            "Name": "LPC",
            "Email": "lpc@gmail.com",
            "Username": "CPL",
            "Address": "Jaipur",
            "Phone": "9999900000"
            ]
        
        CleverTap.sharedInstance()?.onUserLogin(login)
        // Do any additional setup after loading the view.
        
        let update: Dictionary<String, String> = [
            "Name": "LPC",
            "Email": "lpc1998@gmail.com",
            ]
        
        CleverTap.sharedInstance()?.profilePush(update)
        
        CleverTap.sharedInstance()?.recordEvent("Added to Cart")
        CleverTap.sharedInstance()?.recordEvent("Charged")*/
    }


}


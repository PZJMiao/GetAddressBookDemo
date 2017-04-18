# GetAddressBookDemo
app原生获取通讯录的两种方法(a、获取手机通讯录，自己写控件进行展示。b、直接调用系统通讯录，从中选取号码)
- 此demo中包含了获取手机通讯录的两种方法，代码都分别在不同的vc中展示出了。
### 获取手机通讯录，自己写控件进行展示
- 代码在CustomAddressBookVC 中
- 引入几个库：AddressBook.framework、Contacts.framework、ContactsUI.framework
- 引入头文件

```
#import <AddressBook/AddressBook.h>
#import <ContactsUI/ContactsUI.h>
```

- 具体实现方法参考vc中所写

### 直接调用系统通讯录，从中选号码
- 代码在AddressBookVC中（界面展示出来后是系统通讯录的样式）
- 引入库：AddressBook.framework、AddressBookUI.framework、Contacts.framework、ContactsUI.framework
- 引入头文件

```
#import <AddressBookUI/ABPeoplePickerNavigationController.h>
#import <AddressBook/ABPerson.h>
#import <Contacts/Contacts.h>
#import <Contacts/ContactsDefines.h>
#import <ContactsUI/CNContactPickerViewController.h>
#import <ContactsUI/CNContactViewController.h>
#import <ContactsUI/ContactsUI.h>

遵循几个代理（因为系统不同对应的方法也不同）<CNContactPickerDelegate,ABPeoplePickerNavigationControllerDelegate>

```

- 具体实现方法参考vc中所写


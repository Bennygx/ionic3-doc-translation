Action Sheets

Action Sheets���豸��Ļ�ײ���Ե����������ʾһЩ��ȷ�ϻ�ȡ�����ܵ�ѡ�Action Sheets����������˵���Ȼ��Ҫ��������Ϊ����ʹ�á�

ActionSheets���ǳ�����ҳ�����������֮�ϣ����ұ��뱻���ص��Ա��û��ܺ�����������ݽ�������ActionSheets���ֵ�ʱ��ҳ������䰵���Ա�ͻ��ActionSheets��

������Ϣ��鿴API�ĵ���

#����ʹ��#
import { ActionSheetController } from 'ionic-angular';

export class MyPage {
  constructor(public actionSheetCtrl: ActionSheetController) {
  }

  presentActionSheet() {
    let actionSheet = this.actionSheetCtrl.create({
      title: 'Modify your album',
      buttons: [
        {
          text: 'Destructive',
          role: 'destructive',
          handler: () => {
            console.log('Destructive clicked');
          }
        },{
          text: 'Archive',
          handler: () => {
            console.log('Archive clicked');
          }
        },{
          text: 'Cancel',
          role: 'cancel',
          handler: () => {
            console.log('Cancel clicked');
          }
        }
      ]
    });
    actionSheet.present();
  }
}
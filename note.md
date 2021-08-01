 Alert(

        style: AlertStyle(
          animationType: AnimationType.grow,
          animationDuration: Duration(milliseconds: 800),
          isCloseButton: false,
          isOverlayTapDismiss: false,),
        context: context,
        type: AlertType.info,
        title: "TopUp Value : RM"+topupValue.text,
        desc: "xxxxxxxxx",
        buttons: [
          DialogButton(
            child: Text(
              "Cancel",
              style: TextStyle(color: Colors.white, fontSize: 20),
            ),
            onPressed: () => Navigator.pop(context),
            color: Color.fromRGBO(0, 179, 134, 1.0),
          ),
          DialogButton(
            child: Text(
              "Proceed",
              style: TextStyle(color: Colors.white, fontSize: 20),
            ),
            onPressed: (){
              //navigation page here
            },
            color: primary,
          )
        ],
      ).show();

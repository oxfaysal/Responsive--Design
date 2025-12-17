# Responsive App

### Device Size

```
  int pixel4 = 353;
  int samsungs8 = 360;
  int iphone12 = 390;
  int pixel7 = 412;
  int iphone14 = 430;
  int sm = 576;
  int ipadmini = 768;
  int ipadair = 820;
  int surfacepro = 912;
  int lg = 992;
  int ipadpro = 1024;
  int xl = 1200;
  int xxl = 1400;
```


### Responsive AppBar
```
appBar: AppBar(
        title: LayoutBuilder(
          builder: (BuildContext context, BoxConstraints constracints) {
            if (constracints.maxWidth < pixel4) {
              return Text("Mobile");
            } else {
              return Row(
                children: [
                  Row(
                    children: [
                      Image.network(
                        "https://avatars.githubusercontent.com/u/248434219",
                        height: 36,
                      ),
                      SizedBox(width: 6),
                      Text(
                        "Faysal",
                        style: TextStyle(
                          color: Colors.black,
                          fontWeight: FontWeight.w600,
                        ),
                      ),
                    ],
                  ),

                  Spacer(),

                  Row(
                    children: [
                      Text("হোম"),
                      SizedBox(width: 10,),
                      Text("সিডি এটিএস"),
                      SizedBox(width: 10,),
                      Text("সম্পর্কে"),
                      SizedBox(width: 10,),
                      Text("কোর্স"),
                      SizedBox(width: 10,),
                      Text("যোগাযোগ"),
                      SizedBox(width: 10,),
                      Text("কমিউনিটি"),
                    ],
                  ),

                  Spacer(),

                  ElevatedButton(onPressed: (){}, child: Text("SignUp"))
                ],
              );
            }
          },
        ),
      ),

```




###### © All right reserve by Faysal

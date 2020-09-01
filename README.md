# jyWeather
获取所在地实时天气的插件，同时也可获取定位
#使用方式
首先去和风天气申请一个开发者账号 获取对应的key
JYWeather myWeather = new JYWeather(this.getActivity(),"");
        new Thread(new Runnable() {
            @Override
            public void run() {
                String weather = myWeather.getWeather();
                Log.d("weather",weather);
            }
        }).start();
        具体使用可自行使用

# CircleTextProgressbar

����ܵ���ҳ: http://www.yanzhenjie.com
����ܵĲ���: http://blog.csdn.net/yanzhenjie1003

----
# Ч��Ԥ��
<image src="./image/demo.gif" width="350px"/>

#�����ʹ��
������һ��TextView������TextView�Ļ������������С�

��Ϊʵ����̫���ˣ�����չʾ����ô�������ԣ�
```java
// ��ϵͳ��ͨ������һ����0-100��
progressBar.setProgressType(CircleTextProgressbar.ProgressType.COUNT);

// �ı��������
progressBar.setProgressLineWidth(30);// ��������ȡ�
progressBar.setProgressLineWidth(3);// д���ȡ�

// ���õ���ʱʱ����룬Ĭ��3000���롣
progressBar.setTimeMillis(3500);

// �ı��������ɫ��
progressBar.setProgressColor(Color.RED);

// �ı��ⲿ�߿���ɫ��
progressBar.setOutLineColor(Color.RED);

// �ı�Բ����ɫ��
progressBar.setInCircleColor(Color.RED);

// ģ����������������
progressBar.setOutLineColor(Color.TRANSPARENT);// �ⲿ����͸����
progressBar.setInCircleColor(Color.parseColor("#AAC6C6C6"));// �м�ԲΪ��ɫ��
progressBar.setProgressColor(Color.DKGRAY);// ������Ϊ��ɫ��
progressBar.setProgressLineWidth(3); // ���������Ϊ3��
```

���ȼ���
```java
// �������ȡ�
progressBar1.setCountdownProgressListener(1, progressListener);
progressBar2.setCountdownProgressListener(2, progressListener);

OnCountdownProgressListener progressListener = new OnCountdownProgressListener() {
    @Override
    public void onProgress(int what, int progress) {
        if (what == 1) {
            progressBar1.setText(progress + "%");
        } else if (what == 2) {
            progressBar2.setText(progress + "%");
        }
        // ��������ҳ����������жϽ��ȣ����ȵ���100����0��ʱ�������������������
    }
};
```

[0]: [http://www.yanzhenjie.com]
[0]: [http://blog.csdn.net/yanzhenjie1003]
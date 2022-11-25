# react-inpu-typet-groups

- 仿支付宝微信密码输入框 钉钉验证码输入框

- 使用方法

  #### api
       1:type目前支持两种'line'和'box'
       2:length目前两种长度 4和6
       3:getValue获取组件返回值的方法
  #### 引入

   ```
    import InputGroup from 'react-input-type-groups';
    import 'react-input-type-groups/lib/css/styles.css';

    export class Inputarea extends React.Component {
        constructor(props) {
            super(props);
            this.state = {
            };
            this.getValue = this.getValue.bind(this)
        }
        getValue(value) {
            console.log(value)
        }
        render() {
            return (
              <div>
                <InputGroup
                    getValue={this.getValue}
                    length={4}
                    type={'box'}
                />
                <InputGroup
                    getValue={this.getValue}
                    length={4}
                    type={'line'}
                />
              </div>
            );
        }
    }
    ```

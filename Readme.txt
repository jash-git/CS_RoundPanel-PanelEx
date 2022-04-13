C# WINFORM(表單) 畫面邊框畫線元件&四圓角(RoundPanel&PanelEx)

資料來源:
https://blog.csdn.net/breakbridge/article/details/113403842
https://www.cnblogs.com/JiYF/p/9047559.html

RoundPanel Class

PanelEx Class

Use Code
        private void InitializeComponent()
        {
            this.components = new System.ComponentModel.Container();
            System.ComponentModel.ComponentResourceManager resources = new System.ComponentModel.ComponentResourceManager(typeof(main));
            this.panelEx1 = new CS_VPOS.PanelEx(this.components);
            this.roundPanel1 = new CS_VPOS.RoundPanel();
            this.SuspendLayout();
            // 
            // panelEx1
            // 
            this.panelEx1.BorderColor = System.Drawing.Color.Brown;
            this.panelEx1.BorderSize = 3;
            this.panelEx1.Location = new System.Drawing.Point(47, 26);
            this.panelEx1.Name = "panelEx1";
            this.panelEx1.Size = new System.Drawing.Size(397, 178);
            this.panelEx1.TabIndex = 0;
            // 
            // roundPanel1
            // 
            this.roundPanel1.AllRound = ((uint)(20u));
            //this.roundPanel1.BackColor = System.Drawing.Color.FromArgb(((int)(((byte)(28)))), ((int)(((byte)(74)))), ((int)(((byte)(110)))));
            //this.roundPanel1.BackgroundImage = ((System.Drawing.Image)(resources.GetObject("roundPanel1.BackgroundImage")));
            //this.roundPanel1.BackgroundImageLayout = System.Windows.Forms.ImageLayout.Stretch;
            //this.roundPanel1.BackImgColor = System.Drawing.Color.Transparent;
            this.roundPanel1.BorderColor = System.Drawing.Color.Red;
            this.roundPanel1.BorderStyle = System.Windows.Forms.BorderStyle.FixedSingle;
            this.roundPanel1.BorderWidth = 5;
            //this.roundPanel1.BottomLeftRadius = ((uint)(20u));
            //this.roundPanel1.BottomRightRadius = ((uint)(20u));
            this.roundPanel1.Location = new System.Drawing.Point(507, 187);
            this.roundPanel1.Margin = new System.Windows.Forms.Padding(0);
            this.roundPanel1.Name = "roundPanel1";
            this.roundPanel1.Size = new System.Drawing.Size(859, 443);
            this.roundPanel1.TabIndex = 1;
            //this.roundPanel1.TopLeftRadius = ((uint)(20u));
            //this.roundPanel1.TopRightRadius = ((uint)(20u));
            // 
            // main
            // 
            this.AutoScaleDimensions = new System.Drawing.SizeF(12F, 25F);
            this.AutoScaleMode = System.Windows.Forms.AutoScaleMode.Font;
            this.AutoScroll = true;
            this.BackColor = System.Drawing.Color.FromArgb(((int)(((byte)(28)))), ((int)(((byte)(74)))), ((int)(((byte)(110)))));
            this.ClientSize = new System.Drawing.Size(1920, 1080);
            this.Controls.Add(this.roundPanel1);
            this.Controls.Add(this.panelEx1);
            this.Font = new System.Drawing.Font("微軟正黑體", 12F, System.Drawing.FontStyle.Regular, System.Drawing.GraphicsUnit.Point);
            this.FormBorderStyle = System.Windows.Forms.FormBorderStyle.None;
            this.Margin = new System.Windows.Forms.Padding(4);
            this.Name = "main";
            this.Text = "Form1";
            this.WindowState = System.Windows.Forms.FormWindowState.Maximized;
            this.ResumeLayout(false);

        }
        private PanelEx panelEx1;
        private RoundPanel roundPanel1;
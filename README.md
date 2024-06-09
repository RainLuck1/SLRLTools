# SLRLTools
SLRLTools_tools to simplify editing and updating.
        ////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
        // delete xaml
        //    Title="delete" Height="148" Width="307">
        //<Grid>
        //    <TextBox HorizontalAlignment = "Left" Margin="153,39,0,0" TextWrapping="Wrap" Text="" VerticalAlignment="Top" Width="120" x:Name="textbox1" Background="White"/>
        //    <Button Content = "Удалить" HorizontalAlignment="Left" Margin="30,81,0,0" VerticalAlignment="Top" Width="103" Click="Button_Click_1"/>
        //    <Button Content = "Закрыть" HorizontalAlignment="Left" Margin="186,81,0,0" VerticalAlignment="Top" Width="87" Click="Button_Click"/>
        //    <Label Content = "1" HorizontalAlignment="Left" Margin="30,37,0,0" VerticalAlignment="Top" FontSize="14" Name="label"/>
        //</Grid>

        ////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
        // delete xaml cs
        //public partial class delete : Window
        //{
        //public delete()
        //{
        //    InitializeComponent();
        //}

        //private void Button_Click(object sender, RoutedEventArgs e)
        //{
        //    Close();
        //}

        //private void Button_Click_1(object sender, RoutedEventArgs e)
        //{
        //    try
        //    {
        //        SqlConnection conn = new SqlConnection();
        //        conn.ConnectionString = ConfigurationManager.ConnectionStrings["connZay"].ConnectionString;
        //        conn.Open();
        //        SqlCommand cmd = new SqlCommand();
        //        cmd.CommandText = "delete from Zayavka where ID_za = @tb1";
        //        cmd.Parameters.AddWithValue("@tb1", Convert.ToInt32(textbox1.Text));
        //        cmd.Connection = conn;
        //        if (MessageBox.Show("Вы точно хотите удалить эту запись?", "Подтверждение", MessageBoxButton.YesNo, MessageBoxImage.Question) == MessageBoxResult.Yes)
        //        {
        //            int a = cmd.ExecuteNonQuery();
        //            if (a == 1)
        //            {
        //                MessageBox.Show("Успешное удаление данных");
        //            }
        //        }
        //    }
        //    catch
        //    {
        //        MessageBox.Show("Ошибка удаления данных");
        //    }


        //    delete delete = new delete();
        //    delete.Close();
        //}
        //}

        ////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
        // MainWindow xaml
        //Title="MainWindow" Height="450" Width="800">
        //<Grid>
        //    <!--<add name = "connZay" connectionString="Data Source=42-12\SQLEXPRESS;User ID = SA; Password = 1234;Initial Catalog = dmsa;"/>-->
        //    <DataGrid Name = "dg1" AutoGenerateColumns="False" Margin="10,146,10,10" IsReadOnly="True" CanUserAddRows="False">
        //        <DataGrid.Columns>
        //            <DataGridTextColumn Binding = "{Binding ID_oper}" Header="ID оператора" Width="100"/>
        //            <DataGridTextColumn Binding = "{Binding Imya_op}" Header="ФИО опертора" Width="300"/>
        //            <DataGridTextColumn Binding = "{Binding Nomer_op}" Header="Номер телефона" Width="180"/>
        //            <!--<DataGridTextColumn Binding = "{Binding God_poyavlenia, StringFormat='dd.MM.yyyy'}" Header="Дата пояления" Width="100" x:Name="dgc6"/>-->
        //        </DataGrid.Columns>
        //    </DataGrid>

        //    <DataGrid Name = "dg2" AutoGenerateColumns="False" Margin="10,146,10,10" IsReadOnly="True" CanUserAddRows="False">
        //        <DataGrid.Columns>
        //            <DataGridTextColumn Binding = "{Binding ID_rab}" Header="ID работника" Width="100"/>
        //            <DataGridTextColumn Binding = "{Binding Imya_rab}" Header="ФИО работника" Width="300"/>
        //            <DataGridTextColumn Binding = "{Binding Nomer_rab}" Header="Номер телефона" Width="180"/>
        //        </DataGrid.Columns>
        //    </DataGrid>

        //    <DataGrid Name = "dg3" AutoGenerateColumns="False" Margin="10,146,10,10" IsReadOnly="True" CanUserAddRows="False">
        //        <DataGrid.Columns>
        //            <DataGridTextColumn Binding = "{Binding ID_za}" Header="ID заявки" Width="100"/>
        //            <DataGridTextColumn Binding = "{Binding ID_oper}" Header="ID оператора" Width="300"/>
        //            <DataGridTextColumn Binding = "{Binding Opisanie}" Header="Описание" Width="180"/>
        //        </DataGrid.Columns>
        //    </DataGrid>

        //    <DataGrid Name = "dg4" AutoGenerateColumns="False" Margin="10,146,10,10" IsReadOnly="True" CanUserAddRows="False">
        //        <DataGrid.Columns>
        //            <DataGridTextColumn Binding = "{Binding ID_za}" Header="ID заявки" Width="100"/>
        //            <DataGridTextColumn Binding = "{Binding Tip_ustr}" Header="Тип устройства" Width="300"/>
        //            <DataGridTextColumn Binding = "{Binding Model_ustr}" Header="Модель устройства" Width="180"/>
        //            <DataGridTextColumn Binding = "{Binding Data_dob, StringFormat='dd.MM.yyyy'}" Header="Дата добавления" Width="180"/>
        //            <DataGridTextColumn Binding = "{Binding Opisanie}" Header="Описание" Width="180"/>
        //            <DataGridTextColumn Binding = "{Binding FIO_zakazchika}" Header="ФИО заказчика" Width="180"/>
        //            <DataGridTextColumn Binding = "{Binding Nomer_telefona}" Header="Номер телефона" Width="180"/>
        //            <DataGridTextColumn Binding = "{Binding Status_zayavki}" Header="Статус заявки" Width="180"/>
        //            <DataGridTextColumn Binding = "{Binding ID_rabot}" Header="Техник" Width="180"/>
        //        </DataGrid.Columns>
        //    </DataGrid>

        //    <DataGrid Name = "dg5" AutoGenerateColumns="False" Margin="10,146,10,10" IsReadOnly="True" CanUserAddRows="False">
        //        <DataGrid.Columns>
        //            <DataGridTextColumn Binding = "{Binding ID_rab}" Header="ID работника" Width="300"/>
        //            <DataGridTextColumn Binding = "{Binding ID_za}" Header="ID заявки" Width="100"/>
        //        </DataGrid.Columns>
        //    </DataGrid>

        //    <DataGrid Name = "dg6" AutoGenerateColumns="False" Margin="10,146,10,10" IsReadOnly="True" CanUserAddRows="False">
        //        <DataGrid.Columns>
        //            <DataGridTextColumn Binding = "{Binding ID_rab}" Header="ID работника" Width="100"/>
        //            <DataGridTextColumn Binding = "{Binding ID_za}" Header="ID заявки" Width="300"/>
        //            <DataGridTextColumn Binding = "{Binding Rezultat}" Header="Результат" Width="300"/>
        //        </DataGrid.Columns>
        //    </DataGrid>

        //    <DataGrid Name = "dg7" Margin="291,14,291,304" AutoGenerateColumns="False" IsReadOnly="True" CanUserAddRows="False">
        //        <DataGrid.Columns>
        //            <DataGridTextColumn Binding = "{Binding ID_za}" Header="Номер заявки" Width="90"/>
        //            <DataGridTextColumn Binding = "{Binding Status_zayavki}" Header="Завершенные заявки"/>
        //        </DataGrid.Columns>
        //    </DataGrid>

        //    <ComboBox HorizontalAlignment = "Left" Margin="10,10,0,0" VerticalAlignment="Top" Width="120" SelectionChanged="cb1_SelectionChanged" Name="cb1">
        //        <ComboBoxItem Content = "Оператор" Name="Oper"/>
        //        <ComboBoxItem Content = "Работник" Name="Rab"/>
        //        <ComboBoxItem Content = "Регистрация заявки" Name="R_za" />
        //        <ComboBoxItem Content = "Заявка" Name="Za"/>
        //        <ComboBoxItem Content = "Обработка заявки" Name="O_za"/>
        //        <ComboBoxItem Content = "Исполнение заявки" Name="I_za"/>
        //    </ComboBox>
        //    <Button x:Name="b1" Content="Добавить" Margin="603,10,10,0" VerticalAlignment="Top" Height="22" Click="Button_Click"/>
        //    <Button x:Name="b2" Content="Редактировать" Margin="603,37,10,0" VerticalAlignment="Top" Click="Button_Click_2"/>
        //    <Button x:Name="b3" Content="Удалить" Margin="603,62,10,0" VerticalAlignment="Top" Click="Button_Click_1"/>
        //    <Button Content = "Обновить" Click="Button_Click_3" Margin="603,87,10,0" VerticalAlignment="Top"/>

        //</Grid>

        ////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
        // MainWindow xaml cs
        //public partial class MainWindow : Window
        //{
        //public static string table;
        //public MainWindow()
        //{
        //    InitializeComponent();

        //    zapol_dg1();
        //    zapol_dg2();
        //    zapol_dg3();
        //    zapol_dg4();
        //    zapol_dg5();
        //    zapol_dg6();
        //    zapol_dg7();

        //    dg2.Visibility = Visibility.Collapsed;
        //    dg3.Visibility = Visibility.Collapsed;
        //    dg4.Visibility = Visibility.Collapsed;
        //    dg5.Visibility = Visibility.Collapsed;
        //    dg6.Visibility = Visibility.Collapsed;
        //    dg2.Visibility = Visibility.Collapsed;
        //}

        //private void zapol_dg1()
        //{
        //    SqlConnection conn = new SqlConnection();
        //    conn.ConnectionString = ConfigurationManager.ConnectionStrings["connZay"].ConnectionString;
        //    conn.Open();
        //    SqlCommand cmd = new SqlCommand();
        //    cmd.CommandText = "Select * from Operator";
        //    cmd.Connection = conn;
        //    SqlDataAdapter da1 = new SqlDataAdapter(cmd);
        //    DataTable dt1 = new DataTable("Operator");
        //    da1.Fill(dt1);
        //    dg1.ItemsSource = dt1.DefaultView;
        //}
        //private void zapol_dg2()
        //{
        //    SqlConnection conn = new SqlConnection();
        //    conn.ConnectionString = ConfigurationManager.ConnectionStrings["connZay"].ConnectionString;
        //    conn.Open();
        //    SqlCommand cmd = new SqlCommand();
        //    cmd.CommandText = "Select * from Rabotnik";
        //    cmd.Connection = conn;
        //    SqlDataAdapter da1 = new SqlDataAdapter(cmd);
        //    DataTable dt1 = new DataTable("Rabotnik");
        //    da1.Fill(dt1);
        //    dg2.ItemsSource = dt1.DefaultView;
        //}
        //private void zapol_dg3()
        //{
        //    SqlConnection conn = new SqlConnection();
        //    conn.ConnectionString = ConfigurationManager.ConnectionStrings["connZay"].ConnectionString;
        //    conn.Open();
        //    SqlCommand cmd = new SqlCommand();
        //    cmd.CommandText = "Select * from Reg_zayavki";
        //    cmd.Connection = conn;
        //    SqlDataAdapter da1 = new SqlDataAdapter(cmd);
        //    DataTable dt1 = new DataTable("Reg_zayavki");
        //    da1.Fill(dt1);
        //    dg3.ItemsSource = dt1.DefaultView;
        //}
        //private void zapol_dg4()
        //{
        //    SqlConnection conn = new SqlConnection();
        //    conn.ConnectionString = ConfigurationManager.ConnectionStrings["connZay"].ConnectionString;
        //    conn.Open();
        //    SqlCommand cmd = new SqlCommand();
        //    cmd.CommandText = "Select * from Zayavka";
        //    cmd.Connection = conn;
        //    SqlDataAdapter da1 = new SqlDataAdapter(cmd);
        //    DataTable dt1 = new DataTable("Zayavka");
        //    da1.Fill(dt1);
        //    dg4.ItemsSource = dt1.DefaultView;
        //}
        //private void zapol_dg5()
        //{
        //    SqlConnection conn = new SqlConnection();
        //    conn.ConnectionString = ConfigurationManager.ConnectionStrings["connZay"].ConnectionString;
        //    conn.Open();
        //    SqlCommand cmd = new SqlCommand();
        //    cmd.CommandText = "Select * from Obrabotka_zayavki";
        //    cmd.Connection = conn;
        //    SqlDataAdapter da1 = new SqlDataAdapter(cmd);
        //    DataTable dt1 = new DataTable("Obrabotka_zayavki");
        //    da1.Fill(dt1);
        //    dg5.ItemsSource = dt1.DefaultView;
        //}
        //private void zapol_dg6()
        //{
        //    SqlConnection conn = new SqlConnection();
        //    conn.ConnectionString = ConfigurationManager.ConnectionStrings["connZay"].ConnectionString;
        //    conn.Open();
        //    SqlCommand cmd = new SqlCommand();
        //    cmd.CommandText = "Select * from Ispolnenie_zayavki";
        //    cmd.Connection = conn;
        //    SqlDataAdapter da1 = new SqlDataAdapter(cmd);
        //    DataTable dt1 = new DataTable("Ispolnenie_zayavki");
        //    da1.Fill(dt1);
        //    dg6.ItemsSource = dt1.DefaultView;
        //}
        //private void zapol_dg7()
        //{
        //    SqlConnection conn = new SqlConnection();
        //    conn.ConnectionString = ConfigurationManager.ConnectionStrings["connZay"].ConnectionString;
        //    conn.Open();
        //    SqlCommand cmd = new SqlCommand();
        //    cmd.CommandText = "Select ID_za, Status_zayavki from Zayavka where Status_zayavki = 'готова к выдаче' order by ID_za desc";
        //    cmd.Connection = conn;
        //    SqlDataAdapter da1 = new SqlDataAdapter(cmd);
        //    DataTable dt1 = new DataTable("Zayavka");
        //    da1.Fill(dt1);
        //    dg7.ItemsSource = dt1.DefaultView;
        //}
        //private void cb1_SelectionChanged(object sender, SelectionChangedEventArgs e)
        //{
        //    if (Oper.IsSelected)
        //    {
        //        dg1.Visibility = Visibility.Visible;
        //        dg2.Visibility = Visibility.Collapsed;
        //        dg3.Visibility = Visibility.Collapsed;
        //        dg4.Visibility = Visibility.Collapsed;
        //        dg5.Visibility = Visibility.Collapsed;
        //        dg6.Visibility = Visibility.Collapsed;
        //    }
        //    if (Rab.IsSelected)
        //    {
        //        dg1.Visibility = Visibility.Collapsed;
        //        dg2.Visibility = Visibility.Visible;
        //        dg3.Visibility = Visibility.Collapsed;
        //        dg4.Visibility = Visibility.Collapsed;
        //        dg5.Visibility = Visibility.Collapsed;
        //        dg6.Visibility = Visibility.Collapsed;
        //    }
        //    if (R_za.IsSelected)
        //    {
        //        dg1.Visibility = Visibility.Collapsed;
        //        dg2.Visibility = Visibility.Collapsed;
        //        dg3.Visibility = Visibility.Visible;
        //        dg4.Visibility = Visibility.Collapsed;
        //        dg5.Visibility = Visibility.Collapsed;
        //        dg6.Visibility = Visibility.Collapsed;
        //    }
        //    if (Za.IsSelected)
        //    {
        //        dg1.Visibility = Visibility.Collapsed;
        //        dg2.Visibility = Visibility.Collapsed;
        //        dg3.Visibility = Visibility.Collapsed;
        //        dg4.Visibility = Visibility.Visible;
        //        dg5.Visibility = Visibility.Collapsed;
        //        dg6.Visibility = Visibility.Collapsed;
        //    }
        //    if (O_za.IsSelected)
        //    {
        //        dg1.Visibility = Visibility.Collapsed;
        //        dg2.Visibility = Visibility.Collapsed;
        //        dg3.Visibility = Visibility.Collapsed;
        //        dg4.Visibility = Visibility.Collapsed;
        //        dg5.Visibility = Visibility.Visible;
        //        dg6.Visibility = Visibility.Collapsed;
        //    }
        //    if (I_za.IsSelected)
        //    {
        //        dg1.Visibility = Visibility.Collapsed;
        //        dg2.Visibility = Visibility.Collapsed;
        //        dg3.Visibility = Visibility.Collapsed;
        //        dg4.Visibility = Visibility.Collapsed;
        //        dg5.Visibility = Visibility.Collapsed;
        //        dg6.Visibility = Visibility.Visible;
        //    }
        //}

        //private void Button_Click(object sender, RoutedEventArgs e)
        //{
        //    insert insert = new insert();
        //    insert.Show();

        //    insert.label1.Content = "ID заявки";
        //    insert.label2.Content = "Дата добавления";
        //    insert.label3.Content = "Тип устройства";
        //    insert.label4.Content = "Модель устройства";
        //    insert.label5.Content = "Описание проблемы";
        //    insert.label6.Content = "ФИО заказчика";
        //    insert.label7.Content = "Номер телефона";
        //    insert.label8.Content = "Статус заявки";
        //    insert.label9.Content = "Техник";
        //}
        //private void Button_Click_2(object sender, RoutedEventArgs e)
        //{
        //    update update = new update();
        //    update.Show();

        //    update.label1.Content = "ID заявки";
        //    update.label2.Content = "Статус заявки";
        //    update.label3.Content = "Описание проблемы";
        //    update.label4.Content = "Ответственный";
        //}

        //private void Button_Click_1(object sender, RoutedEventArgs e)
        //{
        //    delete delete = new delete();
        //    delete.Show();

        //    delete.label.Content = "ID заявки";
        //}

        //private void Button_Click_3(object sender, RoutedEventArgs e)
        //{
        //    SqlConnection conn = new SqlConnection();
        //    conn.ConnectionString = ConfigurationManager.ConnectionStrings["connZay"].ConnectionString;
        //    conn.Open();

        //    SqlCommand cmd = new SqlCommand();
        //    cmd.Connection = conn;

        //    cmd.CommandText = "Select * from Operator";
        //    SqlDataAdapter da1 = new SqlDataAdapter(cmd);
        //    DataTable dt1 = new DataTable("Operator");
        //    da1.Fill(dt1);
        //    dg1.ItemsSource = dt1.DefaultView;

        //    cmd.CommandText = "Select * from Rabotnik";
        //    SqlDataAdapter da2 = new SqlDataAdapter(cmd);
        //    DataTable dt2 = new DataTable("Rabotnik");
        //    da2.Fill(dt2);
        //    dg2.ItemsSource = dt2.DefaultView;

        //    cmd.CommandText = "Select * from Reg_zayavki";
        //    SqlDataAdapter da3 = new SqlDataAdapter(cmd);
        //    DataTable dt3 = new DataTable("Reg_zayavki");
        //    da3.Fill(dt3);
        //    dg3.ItemsSource = dt3.DefaultView;

        //    cmd.CommandText = "Select * from Zayavka";
        //    SqlDataAdapter da4 = new SqlDataAdapter(cmd);
        //    DataTable dt4 = new DataTable("Zayavka");
        //    da4.Fill(dt4);
        //    dg4.ItemsSource = dt4.DefaultView;

        //    cmd.CommandText = "Select * from Obrabotka_zayavki";
        //    SqlDataAdapter da5 = new SqlDataAdapter(cmd);
        //    DataTable dt5 = new DataTable("Obrabotka_zayavki");
        //    da5.Fill(dt5);
        //    dg5.ItemsSource = dt5.DefaultView;

        //    cmd.CommandText = "Select * from Ispolnenie_zayavki";
        //    SqlDataAdapter da6 = new SqlDataAdapter(cmd);
        //    DataTable dt6 = new DataTable("Ispolnenie_zayavki");
        //    da6.Fill(dt6);
        //    dg6.ItemsSource = dt6.DefaultView;

        //    cmd.CommandText = "Select ID_za, Status_zayavki from Zayavka where Status_zayavki = 'готова к выдаче' order by ID_za desc";
        //    SqlDataAdapter da7 = new SqlDataAdapter(cmd);
        //    DataTable dt7 = new DataTable("Zayavka");
        //    da7.Fill(dt7);
        //    dg7.ItemsSource = dt7.DefaultView;

        //    conn.Close();
        //}
        //}

        ////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
        //insert xaml
        //    Title="insert" Height="450" Width="362">
        //<Grid>
        //    <TextBox Height = "27" Margin="223,15,19,0" TextWrapping="Wrap" Text="" VerticalAlignment="Top" x:Name="textbox1" Background="White"/>
        //    <TextBox Height = "27" Margin="223,43,19,0" TextWrapping="Wrap" Text="" VerticalAlignment="Top" x:Name="textbox2" Background="White"/>
        //    <TextBox Height = "27" Margin="223,71,19,0" TextWrapping="Wrap" Text="" VerticalAlignment="Top" x:Name="textbox3" Background="White"/>
        //    <TextBox Height = "27" Margin="223,99,19,0" TextWrapping="Wrap" Text="" VerticalAlignment="Top" RenderTransformOrigin="0.167,1.304" x:Name="textbox4" Background="White"/>
        //    <TextBox Height = "27" Margin="223,127,19,0" TextWrapping="Wrap" Text="" VerticalAlignment="Top" RenderTransformOrigin="0.167,1.304" x:Name="textbox5" Background="White"/>
        //    <TextBox Height = "27" Margin="223,157,19,0" TextWrapping="Wrap" Text="" VerticalAlignment="Top" RenderTransformOrigin="0.167,1.304" x:Name="textbox6" Background="White"/>
        //    <TextBox Height = "27" Margin="223,186,19,0" TextWrapping="Wrap" Text="" VerticalAlignment="Top" RenderTransformOrigin="0.167,1.304" x:Name="textbox7" Background="White"/>
        //    <Label Content = "1" HorizontalAlignment="Left" Margin="10,15,0,0" VerticalAlignment="Top" FontSize="14" x:Name="label1"/>
        //    <Label Content = "2" HorizontalAlignment="Left" Margin="10,44,0,0" VerticalAlignment="Top" FontSize="14" x:Name="label2"/>
        //    <Label Content = "3" HorizontalAlignment="Left" Margin="10,71,0,0" VerticalAlignment="Top" FontSize="14" x:Name="label3"/>
        //    <Label Content = "4" HorizontalAlignment="Left" Margin="10,99,0,0" VerticalAlignment="Top" FontSize="14" x:Name="label4"/>
        //    <Label Content = "5" HorizontalAlignment="Left" Margin="10,127,0,0" VerticalAlignment="Top" FontSize="14" x:Name="label5"/>
        //    <Label Content = "6" HorizontalAlignment="Left" Margin="10,155,0,0" VerticalAlignment="Top" FontSize="14" x:Name="label6" />
        //    <Label Content = "7" HorizontalAlignment="Left" Margin="10,184,0,0" VerticalAlignment="Top" FontSize="14" x:Name="label7"/>
        //    <Button Content = "Вставить" Margin="19,386,225,0" VerticalAlignment="Top" Click="Button_Click_1"/>
        //    <Button Content = "Закрыть" Margin="223,386,19,0" VerticalAlignment="Top" Click="Button_Click"/>
        //    <TextBox Height = "27" Margin="223,215,19,0" TextWrapping="Wrap" Text="" VerticalAlignment="Top" RenderTransformOrigin="0.167,1.304" x:Name="textbox8" Background="White"/>
        //    <TextBox Height = "27" Margin="223,243,19,0" TextWrapping="Wrap" Text="" VerticalAlignment="Top" RenderTransformOrigin="0.167,1.304" x:Name="textbox9" Background="White"/>

        //    <Label Content = "8" HorizontalAlignment="Left" Margin="10,215,0,0" VerticalAlignment="Top" FontSize="14" x:Name="label8"/>
        //    <Label Content = "9" HorizontalAlignment="Left" Margin="10,243,0,0" VerticalAlignment="Top" FontSize="14" x:Name="label9"/>
        //</Grid>

        ////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
        //insert xaml cs
        //public partial class insert : Window
        //{
        //    public insert()
        //    {
        //        InitializeComponent();
        //    }

        //    private void Button_Click(object sender, RoutedEventArgs e)
        //    {
        //        Close();
        //    }

        //    private void Button_Click_1(object sender, RoutedEventArgs e)
        //    {
        //        try
        //        {
        //            SqlConnection conn = new SqlConnection();
        //            conn.ConnectionString = ConfigurationManager.ConnectionStrings["connZay"].ConnectionString;
        //            conn.Open();
        //            SqlCommand cmd = new SqlCommand();
        //            cmd.CommandText = "INSERT INTO Zayavka (ID_za, Tip_ustr, Model_ustr, Data_dob, Opisanie, FIO_zakazchika, Nomer_telefona, Status_zayavki, ID_rabot) " +
        //                "Values (@tb1,@tb2,@tb3,@tb4,@tb5,@tb6,@tb7,@tb8,@tb9)";
        //            cmd.Parameters.AddWithValue("@tb1", Convert.ToInt32(textbox1.Text));
        //            cmd.Parameters.AddWithValue("@tb2", textbox2.Text);
        //            cmd.Parameters.AddWithValue("@tb3", textbox3.Text);
        //            cmd.Parameters.AddWithValue("@tb4", textbox4.Text);
        //            cmd.Parameters.AddWithValue("@tb5", textbox5.Text);
        //            cmd.Parameters.AddWithValue("@tb6", textbox6.Text);
        //            cmd.Parameters.AddWithValue("@tb7", textbox7.Text);
        //            cmd.Parameters.AddWithValue("@tb8", textbox8.Text);
        //            cmd.Parameters.AddWithValue("@tb9", textbox9.Text);
        //            cmd.Connection = conn;

        //            if (MessageBox.Show("Вы точно хотите добавить эту запись?", "Подтверждение", MessageBoxButton.YesNo, MessageBoxImage.Question) == MessageBoxResult.Yes)
        //            {
        //                int a = cmd.ExecuteNonQuery();
        //                if (a == 1)
        //                {
        //                    MessageBox.Show("Успешное добавление данных");
        //                }
        //            }
        //            //else
        //            //{
        //            //    // Если пользователь отменил добавление, выводим сообщение
        //            //    MessageBox.Show("Добавление отменено");
        //            //}
        //        }
        //        catch
        //        {
        //            MessageBox.Show("Ошибка добавления данных");
        //        }


        //        insert insert = new insert();
        //        insert.Close();
        //    }
        //}

        ////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
        //update xaml
        //    Title="update" Height="218" Width="376">
        //<Grid Height = "173" VerticalAlignment="Top">
        //    <TextBox Height = "27" Margin="223,15,19,0" TextWrapping="Wrap" Text="" VerticalAlignment="Top" x:Name="textbox1" Background="White"/>
        //    <TextBox Height = "27" Margin="223,43,19,0" TextWrapping="Wrap" Text="" VerticalAlignment="Top" x:Name="textbox2" Background="White"/>
        //    <TextBox Height = "27" Margin="223,71,19,0" TextWrapping="Wrap" Text="" VerticalAlignment="Top" RenderTransformOrigin="0.167,1.304" x:Name="textbox3" Background="White"/>
        //    <TextBox Height = "27" Margin="223,100,19,0" TextWrapping="Wrap" Text="" VerticalAlignment="Top" RenderTransformOrigin="0.167,1.304" x:Name="textbox4" Background="White"/>
        //    <Label Content = "1" HorizontalAlignment="Left" Margin="10,15,0,0" VerticalAlignment="Top" FontSize="14" x:Name="label1"/>
        //    <Label Content = "2" HorizontalAlignment="Left" Margin="10,44,0,0" VerticalAlignment="Top" FontSize="14" x:Name="label2"/>
        //    <Label Content = "3" HorizontalAlignment="Left" Margin="10,71,0,0" VerticalAlignment="Top" FontSize="14" x:Name="label3"/>
        //    <Label Content = "4" HorizontalAlignment="Left" Margin="10,98,0,0" VerticalAlignment="Top" FontSize="14" x:Name="label4"/>
        //    <Button Content = "Обновить" Margin="19,143,225,10" Click="Button_Click_1"/>
        //    <Button Content = "Закрыть" Margin="223,143,19,10" Click="Button_Click"/>
        //</Grid>

        ////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
        //update xaml cs
        //public partial class update : Window
        //{
        //    public update()
        //    {
        //        InitializeComponent();
        //    }

        //    private void Button_Click(object sender, RoutedEventArgs e)
        //    {
        //        Close();
        //    }

        //    private void Button_Click_1(object sender, RoutedEventArgs e)
        //    {
        //        try
        //        {
        //            SqlConnection conn = new SqlConnection();
        //            conn.ConnectionString = ConfigurationManager.ConnectionStrings["connZay"].ConnectionString;
        //            conn.Open();
        //            SqlCommand cmd = new SqlCommand();
        //            cmd.CommandText = "UPDATE Zayavka SET ID_za = @tb1, Status_zayavki = @tb2, Opisanie = @tb3, ID_rabot = @tb4 where ID_za = @tb1";
        //            cmd.Parameters.AddWithValue("@tb1", Convert.ToInt32(textbox1.Text));
        //            cmd.Parameters.AddWithValue("@tb2", textbox2.Text);
        //            cmd.Parameters.AddWithValue("@tb3", textbox3.Text);
        //            cmd.Parameters.AddWithValue("@tb4", textbox4.Text);
        //            cmd.Connection = conn;
        //            if (MessageBox.Show("Вы точно хотите обновить эту запись?", "Подтверждение", MessageBoxButton.YesNo, MessageBoxImage.Question) == MessageBoxResult.Yes)
        //            {
        //                int a = cmd.ExecuteNonQuery();
        //                if (a == 1)
        //                {
        //                    MessageBox.Show("Успешное обновление данных");
        //                }
        //            }
        //        }
        //        catch
        //        {
        //            MessageBox.Show("Ошибка обновления данных");
        //        }


        //        insert insert = new insert();
        //        insert.Close();
        //    }
        //}

        ////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
        //Window xaml
        //    Title="Вход" Height="170" Width="268">
        //<Grid>
        //    <TextBox HorizontalAlignment = "Left" Margin="117,25,0,0" TextWrapping="Wrap" Text="Admin" VerticalAlignment="Top" Width="120" Name="tb1"/>
        //    <TextBox HorizontalAlignment = "Left" Margin="117,55,0,0" TextWrapping="Wrap" Text="1234" VerticalAlignment="Top" Width="120" Name="tb2"/>
        //    <Label Content = "Логин" HorizontalAlignment="Left" Margin="27,21,0,0" VerticalAlignment="Top"/>
        //    <Label Content = "Пароль" HorizontalAlignment="Left" Margin="27,51,0,0" VerticalAlignment="Top"/>
        //    <Button Content = "Войти" Margin="168,108,0,0" Click="Button_Click" Height="20" VerticalAlignment="Top" HorizontalAlignment="Left" Width="69"/>
        //    <Button Content = "Выход" Margin="0,108,172,0" Click="Button_Click_1" Height="20" VerticalAlignment="Top" HorizontalAlignment="Right" Width="69"/>
        //</Grid>

        ////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
        //Window xaml cs
        //public partial class Window1 : Window
        //{
        //public Window1()
        //{
        //    InitializeComponent();
        //}

        //private void Button_Click(object sender, RoutedEventArgs e)
        //{
        //    if (tb1.Text == "Admin" && tb2.Text == "1234")
        //    {
        //        MainWindow MainWindow = new MainWindow();
        //        MainWindow.Show();
        //        Close();
        //    }
        //    else if (tb1.Text == "P1" && tb2.Text == "1234")
        //    {
        //        MainWindow MainWindow = new MainWindow();
        //        MainWindow.Show();
        //        MainWindow.b1.IsEnabled = false;
        //        MainWindow.b2.IsEnabled = false;
        //        MainWindow.b3.IsEnabled = false;
        //        Close();
        //    }
        //    else
        //    {
        //        MessageBox.Show("Введен неверный пароль или логин");
        //    }
        //}

        //private void Button_Click_1(object sender, RoutedEventArgs e)
        //{
        //    Close();
        //}
        //}


        //        //ГБПОУ Нефтекамский машиностроительный колледж







        //        СПЕЦИФИКАЦИЯ МОДУЛЯ 
        //«ФОРМИРОВАНИЕ ЗАКАЗА» ДЛЯ ИНФОРМАЦИОННОЙ
        //СИСТЕМЫ ООО «РУЛЬ»















        //Студент: Фамилия Имя Отчество
        //Группа: Группа
        //Специальность: 09.02.07 Информационные системы и программирование


        //Содержание

        //1	Назначение модуля	3
        //2	Входные данные	4
        //3	Выходные данные	5
        //4	Алгоритм работы модуля	6
        //5	Блок-схема	7
        //6	Реализованные функции	8
        //7	Дополнительные требования(Нефункциональные требования) 9


        //1	Назначение модуля

        //Модуль предназначен для формирования заказов на товары, представленные в каталоге информационной системы ООО «Руль», для неавторизованных и авторизованных клиентов с возможностью выбора пункта выдачи заказа. (Брать из описания предметной области)

        //2	Входные данные

        //Основные входные данные, определенные техническим заданием(ТЗ) для программного модуля:
        //–	каталог товаров с информацией о фото, наименовании, описании, производителе, цене и скидке(если применимо);
        //–	данные о клиенте, в случае авторизации: имя, логин, адрес;
        //–	список товаров, выбранных пользователем для заказа;
        //–	количество каждого товара, выбранного пользователем;
        //–	пункта выдачи заказа пользователем.

        //3	Выходные данные

        //Основные выходные данные, определенные ТЗ для программного модуля:
        //–	уникальный номер, автоматически присваиваемый заказу;
        //–	список товаров, добавленных в заказ, с указанием количества, цены, скидки и общей стоимости;
        //–	итоговая стоимость заказа с учетом скидок;
        //–	общая сумма скидки, примененная к товарам в заказе;
        //–	статус заказа(изначально «новый»);
        //–	дата и время создания заказа;
        //–	выбранный пользователем пункт выдачи заказа;
        //–	случайно сгенерированный 3-хзначный код для получения заказа);
        //–	срок доставки(3 дня, если в наличии на складе не менее 3 позиций заказа, 6 дней - в противном случае);
        //–	талон заказа в формате PDF-документа с информацией о заказе, включая дату, номер заказа, состав, сумму, скидку, пункт выдачи и код получения)

        //4	Алгоритм работы модуля

        //1.	Просмотр пользователем списка товаров.
        //2.	Добавление в заказ.
        //2.1.	Пользователь выбирает товар и добавляет его в заказ (кол-во по умолчанию - 1).
        //2.2.	При каждом добавлении товара, обновляется информация о составе заказа, сумме заказа и сумме скидки.
        //3.	Просмотр заказа.
        //4.	Удаление товаров.
        //4.1.	Пользователь может удалить товар из заказа, установив количество товара 0 или нажатием на элемент интерфейса.
        //4.2.	При удалении товара, обновляется информация о составе заказа, сумме заказа и сумме скидки.
        //5.	Выбор пункта выдачи.
        //6.	Создание заказа.
        //6.1.	После выбора пункта выдачи и подтверждения заказа, система автоматически присваивает заказу номер, генерирует код получения, устанавливает статус «Новый» и сохраняет информацию о заказе в базу данных.
        //6.2.	Система рассчитывает срок доставки заказа в зависимости от наличия товаров на складе.
        //7.	Формирование талона заказа.
        //7.1.	Система генерирует PDF-талон с информацией о заказе, включая дату, номер заказа, состав, сумму, скидку, пункт выдачи и код получения.
        //7.2.	Срок доставки указывается в талоне в зависимости от наличия товаров на складе.

        //5	Блок-схема

        //БЛОК СХЕМА ПО ГОСТУ 19.701-90 (90 – год)

        //6	Реализованные функции

        //Функции модуля для успешного удовлетворения требования ТЗ:
        //–	добавление товаров в заказ;
        //–	удаление товаров из заказа;
        //–	просмотр и редактирование состава заказа;
        //–	расчет общей стоимости заказа, суммы скидки и срока доставки;
        //–	выбор пункта выдачи;
        //–	автоматическая генерация номера заказа, кода получения и PDF-талона;
        //–	сохранение информации о заказе в базу данных.

        //7	Дополнительные требования(Нефункциональные требования)

        //Классификация требования, подпадающие под категорию дополнительных требований, исполняемые после успешного исполнения основных требования:
        //–	модуль должен быть реализован с использованием графического интерфейса пользователя(GUI);
        //–	должна быть реализована проверка введенных пользователем данных на корректность;
        //–	информация о заказе должна быть представлена пользователю в удобном и понятном виде;
        //–	модуль должен интегрироваться с остальными модулями информационной системы ООО «Руль».

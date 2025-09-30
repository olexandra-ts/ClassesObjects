using System;
using System.Collections.Generic;
using System.Globalization;
using System.Text;
using System.Windows.Forms;
namespace TsitelashviliLab1
{
public partial class Form1 : Form
{
private readonly List<Perfume> perfumes = new List<Perfume>();
public Form1()
{
InitializeComponent();
}
public class Perfume
{
public string Brand { get; set;}
public string Name { get; set; }
public string Year { get; set; }
public string Notes { get; set; }
public string V olume { get; set; }
public string Price { get; set; }
public string Packaging { get; set; }
private void label2
_
Click(object sender, EventArgs e)
private void label3
private void label5
private void label1
private void Form1
}
{
}
{
}
{
}
{
}
{
}
_
Click(object sender, EventArgs e)
_
Click(object sender, EventArgs e)
_
Click(object sender, EventArgs e)
_
Load(object sender, EventArgs e)
private void pictureBox1
_
Click(object sender, EventArgs e)
private void button1
{
}
{
}
{
_
Click(object sender, EventArgs e)
private void btnAdd
_
Click(object sender, EventArgs e)
Perfume perfume = new Perfume()
{
Brand = txtBrand.Text,
Name = txtName.Text,
Year = txtYear.Text,
Notes = txtNotes.Text,
V olume = txtV olume.Text,
Price = txtPrice.Text,
Packaging = txtPackaging.Text
};
perfumes.Add(perfume);
txtBrand.Clear();
txtName.Clear();
txtYear.Clear();
txtNotes.Clear();
txtV olume.Clear();
txtPrice.Clear();
txtPackaging.Clear();
MessageBox.Show("Парфум додано");
}
{
private void btnShow
_
Click(object sender, EventArgs e)
if (perfumes.Count == 0)
{
MessageBox.Show("Немає збережених парфумів");
return;
}
string result = "";
}
result += $"Бренд: {p.Brand}\n" +
$"Назва: {p.Name}\n" +
$"Рік випуску: {p.Year}\n" +
$"Ноти: {p.Notes}\n" +
$"Об'єм: {p.V olume}\n" +
$"Ціна: {p.Price}\n" +
$"Упаковка: {p.Packaging}\n" +
"
\n";
_______________________________
MessageBox.Show(result,
"Список парфумів ");
}
}
}

# Examen Dispozitive si Aplicatii Mobile <br>

## Cerinta 1
> Se va defini o clasa cu minim cinci atribute relevante, din domeniul dat, pentru care se vor implementa/genera constructori, metoda  *toString()* si functii accesor(metode get(), set()) **(1p)**.

``
public class ClasaExamen {
    private int proprietate_int_1;
    private int proprietate_int_2;
    private String proprietate_string;
    private Date proprietate_date;
    private TipProprietate proprietate_tip;

    public ClasaExamen(int proprietate_int_1, int proprietate_int_2, String proprietate_string, Date proprietate_date, TipProprietate proprietate_tip) {
        this.proprietate_int_1 = proprietate_int_1;
        this.proprietate_int_2 = proprietate_int_2;
        this.proprietate_string = proprietate_string;
        this.proprietate_date = proprietate_date;
        this.proprietate_tip = proprietate_tip;
    }

    public int getProprietate_int_1() {
        return proprietate_int_1;
    }

    public void setProprietate_int_1(int proprietate_int_1) {
        this.proprietate_int_1 = proprietate_int_1;
    }

    public int getProprietate_int_2() {
        return proprietate_int_2;
    }

    public void setProprietate_int_2(int proprietate_int_2) {
        this.proprietate_int_2 = proprietate_int_2;
    }

    public String getProprietate_string() {
        return proprietate_string;
    }

    public void setProprietate_string(String proprietate_string) {
        this.proprietate_string = proprietate_string;
    }

    public Date getProprietate_date() {
        return proprietate_date;
    }

    public void setProprietate_date(Date proprietate_date) {
        this.proprietate_date = proprietate_date;
    }

    public TipProprietate getProprietate_tip() {
        return proprietate_tip;
    }

    public void setProprietate_tip(TipProprietate proprietate_tip) {
        this.proprietate_tip = proprietate_tip;
    }

    @Override
    public String toString() {
        return "ClasaExamen{" +
                "proprietate_int_1=" + proprietate_int_1 +
                ", proprietate_int_2=" + proprietate_int_2 +
                ", proprietate_string='" + proprietate_string + '\'' +
                ", proprietate_date=" + proprietate_date +
                ", proprietate_tip=" + proprietate_tip +
                '}';
    }
}
``
